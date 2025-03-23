# Approach for Masked Autoencoder Pretraining and Classification Fine-tuning

## 1. Pretraining the Masked Autoencoder
We adapted the official implementation of Masked Autoencoders (MAE) and designed a custom architecture trained from scratch. The model follows an **asymmetric encoder-decoder architecture**, ensuring that the encoder learns a dense representation.

### Loss Function
Initially, **Mean Squared Error (MSE) loss** was used for reconstruction, but due to the predominance of low pixel values in images, MSE quickly dropped to zero, making interpretation difficult and leading to poor reconstruction quality. To address this, we switched to **Binary Cross-Entropy with Logits Loss (BCELogit)** on **normalized images**, which resulted in improved visual reconstructions.

### Experimental Setup
We experimented with three different scales of the model:

| Embedding Size | Patch Size | Masking Ratio | Training Epochs (avg) | Final Loss (approx) |
|---------------|-----------|---------------|------------------|----------------|
| 128          | 8         | 0.3           | 300-500          | 0.0062         |
| 256          | 4         | 0.75          | 300-500          | 0.0062         |
| 300          | 4         | 0.75          | 300-500          | 0.0062         |

The models generally converged within **300 to 500 epochs**, reaching a stable loss value of approximately **0.0062** under the current learning rate schedule.

---

## 2. Classification Fine-Tuning
The classification task was tackled using a **two-step fine-tuning** process:
1. **Linear Probing**: Training an MLP adapter layer while keeping the encoder frozen.
2. **Full Fine-Tuning**: Training the entire model with different learning rates for the encoder and the MLP head.

### Step 1: Linear Probing
- An **MLP adapter** is trained to predict classes with a frozen encoder.
- We use **LARS optimizer (self-implemented)** since **AdamW and SGD alone show poor convergence**.
- This phase achieves an accuracy of **40% to 48%** with a **micro-averaged ROC-AUC of ~0.64**.

### Step 2: Full Fine-Tuning
- The entire model is trained with **separate learning rates** for the encoder and the MLP.
- **AdamW optimizer** is used.
- The model is trained for **~150 epochs**, achieving:
  - **85% accuracy** with just **2M parameters**.
  - **Micro-averaged AUC of 0.93**.

### Model Size vs. MLP Depth Trade-off
Shallower encoders require deeper MLP heads, whereas deeper encoders perform well with relatively shallow MLPs.

| Encoder Size | Parameters | MLP Head Size | Parameters |
|-------------|------------|--------------|------------|
| Shallow     | ~1.5M      | Deep         | ~700K      |
| Deep        | Heavier    | Shallow      | ~200K      |

---

## Summary
- A **custom MAE** was trained from scratch with BCELogit loss for better reconstruction.
- **Three architecture variants** were evaluated with different embedding sizes, patch sizes, and masking ratios.
- **Two-stage classification fine-tuning** (Linear Probing + Full Fine-Tuning) was conducted.
- Achieved **85% classification accuracy with 2M parameters** and a **micro-averaged AUC of 0.93**.

This structured approach ensures an efficient model with a balance between accuracy and computational efficiency.

