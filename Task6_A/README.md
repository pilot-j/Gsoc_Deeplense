# Fine-tuning a Pretrained Masked Autoencoder (MAE) for Classification

## Introduction
This project utilizes a pretrained **Masked Autoencoder (MAE)** for image classification on a given dataset. The approach consists of two stages:
1. **Linear Probing:** Training a classification head while keeping the pretrained MAE frozen.
2. **Full Fine-tuning:** Unfreezing the MAE and optimizing all model parameters for better performance.

## Pretraining Details
The MAE model was pretrained in a self-supervised manner by reconstructing masked image patches. Below are the loss curve and sample reconstructed images from pretraining:

### Pretraining Loss Curve
![Pretraining Loss Curve](../images/Task6A/task6A_loss_curve.png)

### Pretraining Output Samples
![Reconstructed Images](../images/Task6A/task6A_pretrain_img_map.png)

## Fine-tuning Approach
### 1. Linear Probing
- The pretrained MAE encoder is **frozen**, and only a newly added classification MLP is trained.
- This step evaluates how well the MAE encoder captures meaningful features.

### 2. Full Fine-tuning
- The entire model, including the MAE encoder, is **unfrozen** and fine-tuned end-to-end.
- This allows the encoder to adapt to the classification task.

### ROC-AUC Curves
#### Linear Probing ROC-AUC
![ROC-AUC Linear Probing](../images/Task6A/task6A_LP_ROC_AUC.png)

#### Full Fine-tuning ROC-AUC
![ROC-AUC Full Fine-tune](../images/Task6A/task6A_FT_ROC_AUC.png)

## Hyperparameters & Training Details
| Phase              | Optimizer  | Learning Rate | Scheduler  | # Parameters |
|-------------------|------------|--------------|------------|-------------|
| Linear Probing    | LARS      | 1e-3 (SGD Base)         | Cosine Annealing | ~200K  |
| Full Fine-tuning  | AdamW      | 9.5e-5 for encoder, 8e-4 for others         | Cosine Annealing | ~6.6M  |



