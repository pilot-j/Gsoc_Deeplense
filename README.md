# Gsoc_Deeplense
Entry for GSoc Deeplense 'Foundational Model' project. Contains jupyter nbs, scripts and results of tasks.
Results for specific task (task 6) can be reproduced by running [validation_nb](validation_deeplense_task6.ipynb) notebook on kaggle

Separate Train Val folders were not provided for task 6 so I have split them into 90:10 ratio.
Dataset links (organised into train val spilts and uploaded on kaggle):
1. [Pretraining and classification finetuning](https://www.kaggle.com/datasets/mldtype/masked-autoencoder)
2. [Super resolution finetuning](https://www.kaggle.com/datasets/mldtype/mae-sr-dataset-split/data)

WEIGHTS(Kaggle) - [official_weights](https://www.kaggle.com/datasets/mldtype/weights-ml4sci-all)
# Consolidated Task Results

This document reports the results of all tasks, collectively presenting key model performance metrics.

## Results Table

|TASK | Model       | # Train Params | Mode     | Metric 
|------------|------------|---------|---------|--------|
| common task| CNN Classifier   | 13.6M     | Training | AUC - 1 for all classes 
| Task6A | Masked AutoEncoder    | 7.25M    | Pre training  | Val loss - ~0.0062 (BCEWithLogitsLoss)
| Task6A| MAE Classifier    | 6.6M    | Probing + Finetuning| Micro-Avg AUC - 0.97  
| Task6B| SuperResolution MAE    | 7.38M    | Full Finetuning | PSNR - 33.6579, SSIM - 0.9681, MSE- 0.00042 
| Task6A | MAE Classifier    | ~200K    | Linear Probing | Micro-avg AUC - 0.58  





## Notes
- The MAE models are kept relatively small (< ~10M parameters) due to computational constraints. This approach has also helped me assess whether small ViT-based models can be effectively fine-tuned. I believe that scaling the encoder to larger dimension sizes would significantly improve the results. From my experimentation with embedding dimensions ranging from 128 to 300, I can anecdotally confirm this trend.
- The reported metric values represent the best performance achieved in the respective modes.
- Further details in task specific folders


