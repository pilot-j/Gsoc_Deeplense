# Gsoc_Deeplense
Entry for GSoc Deeplense 'Foundational Model' project. Contains jupyter nbs, scripts and results of tasks.
Results for specific task (task 6) can be reproduced by running [validation_nb](validation_deeplense_task6.ipynb) notebook on kaggle

Dataset links (organised into train val spilts and uploaded on kaggle):
1. [Pretraining and classification finetuning](https://www.kaggle.com/datasets/mldtype/masked-autoencoder)
2. [Super resolution finetuning](https://www.kaggle.com/datasets/mldtype/mae-sr-dataset-split/data)

WEIGHTS(Kaggle) - [official_weights](https://www.kaggle.com/datasets/mldtype/weights-ml4sci-all)
# Consolidated Task Results

This document reports the results of all tasks, collectively presenting key model performance metrics.

## Results Table

| Model       | # Train Params | Mode     | Metric |TASK
|------------|---------|---------|--------|-------|
| CNN Classifier   | 13.6M     | Training | AUC - 1 for all classes  | common task
| Masked AutoEncoder    | 7.25M    | Pre training  | -| Task6A
| MAE Classifier    | 6.6M    | Probing + Finetuning| Micro-Avg AUC - 0.97  | Task6A
| SuperResolution MAE    | 7.38M    | Full Finetuning | PSNR - 33.6579, SSIM - 0.9681, MSE- 0.00042 | Task6B
| MAE Classifier    | ~200K    | Linear Probing | Micro-avg AUC - 0.58  | Task6A




## Notes
- The reported metric values represent the best performance achieved in the respective modes.
- Further details in task specific folders


