## Training Progress

### Epoch-wise Training and Validation Performance for linear probing with Freezed Encoder

First 50 epochs

```
Epoch 1/50 [LP]: 100%|██████████| 157/157 [03:19<00:00,  1.27s/it, loss=1.14]
Epoch 1/50 [Validating]: 100%|██████████| 18/18 [00:21<00:00,  1.19s/it]

Saving model at Epoch 1 with Validation Accuracy: 36.99%
Epoch 1/50 - Train Loss: 1.1430, Train Accuracy: 33.87%, Validation Loss: 1.0950, Validation Accuracy: 36.99%

Epoch 2/50 [LP]: 100%|██████████| 157/157 [02:23<00:00,  1.10it/s, loss=1.11]
Epoch 2/50 [Validating]: 100%|██████████| 18/18 [00:17<00:00,  1.04it/s]

Saving model at Epoch 2 with Validation Accuracy: 38.46%
Epoch 2/50 - Train Loss: 1.1265, Train Accuracy: 35.09%, Validation Loss: 1.0903, Validation Accuracy: 38.46%

Epoch 3/50 [LP]: 100%|██████████| 157/157 [02:23<00:00,  1.09it/s, loss=1.1]
Epoch 3/50 [Validating]: 100%|██████████| 18/18 [00:15<00:00,  1.13it/s]

Saving model at Epoch 3 with Validation Accuracy: 38.96%
Epoch 3/50 - Train Loss: 1.1208, Train Accuracy: 35.82%, Validation Loss: 1.0887, Validation Accuracy: 38.96%

...

Epoch 30/50 [LP]: 100%|██████████| 157/157 [02:21<00:00,  1.11it/s, loss=1.09]
Epoch 30/50 [Validating]: 100%|██████████| 18/18 [00:15<00:00,  1.20it/s]

Saving model at Epoch 30 with Validation Accuracy: 43.73%
Epoch 30/50 - Train Loss: 1.0793, Train Accuracy: 40.35%, Validation Loss: 1.0599, Validation Accuracy: 43.73%

Epoch 32/50 [LP]: 100%|██████████| 157/157 [02:20<00:00,  1.11it/s, loss=1.09]
Epoch 32/50 [Validating]: 100%|██████████| 18/18 [00:17<00:00,  1.01it/s]

Saving model at Epoch 32 with Validation Accuracy: 43.93%
Epoch 32/50 - Train Loss: 1.0760, Train Accuracy: 40.92%, Validation Loss: 1.0609, Validation Accuracy: 43.93%

...
```

Next 50 Epochs
```
Epoch 1/50 [LP]: 100%|██████████| 157/157 [02:21<00:00,  1.11it/s, loss=1.07]
Epoch 1/50 [Validating]: 100%|██████████| 18/18 [00:15<00:00,  1.14it/s]

Saving model at Epoch 1 with Validation Accuracy: 46.27%
Epoch 1/50 - Train Loss: 1.0451, Train Accuracy: 44.23%, Validation Loss: 1.0324, Validation Accuracy: 46.27%
Epoch 2/50 [LP]: 100%|██████████| 157/157 [02:22<00:00,  1.10it/s, loss=1.04]
Epoch 2/50 [Validating]: 100%|██████████| 18/18 [00:15<00:00,  1.18it/s]
Epoch 2/50 - Train Loss: 1.0459, Train Accuracy: 44.27%, Validation Loss: 1.0386, Validation Accuracy: 45.07%
Epoch 3/50 [LP]: 100%|██████████| 157/157 [02:22<00:00,  1.11it/s, loss=1.07]
Epoch 3/50 [Validating]: 100%|██████████| 18/18 [00:16<00:00,  1.07it/s]
Epoch 3/50 - Train Loss: 1.0444, Train Accuracy: 44.41%, Validation Loss: 1.0381, Validation Accuracy: 45.49%
Epoch 4/50 [LP]: 100%|██████████| 157/157 [02:30<00:00,  1.04it/s, loss=0.99]
Epoch 4/50 [Validating]: 100%|██████████| 18/18 [00:17<00:00,  1.00it/s]
Epoch 4/50 - Train Loss: 1.0439, Train Accuracy: 44.60%, Validation Loss: 1.0397, Validation Accuracy: 45.15%
Epoch 5/50 [LP]: 100%|██████████| 157/157 [02:21<00:00,  1.11it/s, loss=1.05]
Epoch 5/50 [Validating]: 100%|██████████| 18/18 [00:15<00:00,  1.15it/s]
Epoch 5/50 - Train Loss: 1.0429, Train Accuracy: 44.29%, Validation Loss: 1.0317, Validation Accuracy: 45.91%
Epoch 6/50 [LP]: 100%|██████████| 157/157 [02:27<00:00,  1.06it/s, loss=1.06]
Epoch 6/50 [Validating]: 100%|██████████| 18/18 [00:15<00:00,  1.16it/s]

Saving model at Epoch 6 with Validation Accuracy: 46.41%
Epoch 6/50 - Train Loss: 1.0452, Train Accuracy: 44.12%, Validation Loss: 1.0321, Validation Accuracy: 46.41%
Epoch 7/50 [LP]: 100%|██████████| 157/157 [02:21<00:00,  1.11it/s, loss=1.08]
Epoch 7/50 [Validating]: 100%|██████████| 18/18 [00:16<00:00,  1.11it/s]

Saving model at Epoch 7 with Validation Accuracy: 46.43%
.....
Epoch 10/50 - Train Loss: 1.0428, Train Accuracy: 44.39%, Validation Loss: 1.0356, Validation Accuracy: 46.37%
Epoch 11/50 [LP]: 100%|██████████| 157/157 [02:28<00:00,  1.06it/s, loss=1.05]
Epoch 11/50 [Validating]: 100%|██████████| 18/18 [00:16<00:00,  1.09it/s]

Saving model at Epoch 11 with Validation Accuracy: 46.53%
Epoch 11/50 - Train Loss: 1.0444, Train Accuracy: 44.48%, Validation Loss: 1.0309, Validation Accuracy: 46.53%
....
Epoch 14/50 [Validating]: 100%|██████████| 18/18 [00:16<00:00,  1.12it/s]
Epoch 14/50 - Train Loss: 1.0406, Train Accuracy: 44.91%, Validation Loss: 1.0319, Validation Accuracy: 45.94%
Epoch 15/50 [LP]: 100%|██████████| 157/157 [02:25<00:00,  1.08it/s, loss=1.05]
Epoch 15/50 [Validating]: 100%|██████████| 18/18 [00:15<00:00,  1.13it/s]

Saving model at Epoch 15 with Validation Accuracy: 47.08%
Epoch 15/50 - Train Loss: 1.0416, Train Accuracy: 44.65%, Validation Loss: 1.0271, Validation Accuracy: 47.08%
Epoch 16/50 [LP]: 100%|██████████| 157/157 [02:21<00:00,  1.11it/s, loss=1.06]
....
Epoch 20/50 [Validating]: 100%|██████████| 18/18 [00:16<00:00,  1.11it/s]

Saving model at Epoch 20 with Validation Accuracy: 47.50%
Epoch 20/50 - Train Loss: 1.0395, Train Accuracy: 44.75%, Validation Loss: 1.0261, Validation Accuracy: 47.50%
Epoch 21/50 [LP]: 100%|██████████| 157/157 [02:21<00:00,  1.11it/s, loss=1.04]
Epoch 21/50 [Validating]: 100%|██████████| 18/18 [00:14<00:00,  1.21it/s]
Epoch 21/50 - Train Loss: 1.0383, Train Accuracy: 44.94%, Validation Loss: 1.0334, Validation Accuracy: 45.57%

.....
Epoch 33/50 - Train Loss: 1.0346, Train Accuracy: 45.46%, Validation Loss: 1.0269, Validation Accuracy: 47.28%
Epoch 34/50 [LP]: 100%|██████████| 157/157 [02:22<00:00,  1.10it/s, loss=1.06] 
Epoch 34/50 [Validating]: 100%|██████████| 18/18 [00:17<00:00,  1.00it/s]

Saving model at Epoch 34 with Validation Accuracy: 47.54%
Epoch 34/50 - Train Loss: 1.0357, Train Accuracy: 45.06%, Validation Loss: 1.0230, Validation Accuracy: 47.54%
Epoch 38/50 - Train Loss: 1.0361, Train Accuracy: 45.26%, Validation Loss: 1.0240, Validation Accuracy: 47.05%
Epoch 39/50 [LP]: 100%|██████████| 157/157 [02:23<00:00,  1.10it/s, loss=1]    
Epoch 39/50 [Validating]: 100%|██████████| 18/18 [00:15<00:00,  1.18it/s]

Saving model at Epoch 39 with Validation Accuracy: 47.95%
Epoch 39/50 - Train Loss: 1.0367, Train Accuracy: 45.17%, Validation Loss: 1.0207, Validation Accuracy: 47.95%
Epoch 40/50 [LP]: 100%|██████████| 157/157 [02:21<00:00,  1.11it/s, loss=1.07] 
Epoch 40/50 [Validating]: 100%|██████████| 18/18 [00:16<00:00,  1.07it/s]
Epoch 40/50 - Train Loss: 1.0356, Train Accuracy: 45.20%, Validation Loss: 1.0210, Validation Accuracy: 46.83%
Epoch 41/50 [LP]: 100%|██████████| 157/157 [02:22<00:00,  1.10it/s, loss=1.05] 
Epoch 41/50 [Validating]: 100%|██████████| 18/18 [00:15<00:00,  1.15it/s]
Epoch 41/50 - Train Loss: 1.0336, Train Accuracy: 45.36%, Validation Loss: 1.0264, Validation Accuracy: 46.72%
Epoch 42/50 [LP]: 100%|██████████| 157/157 [02:23<00:00,  1.10it/s, loss=0.995]
Epoch 42/50 [Validating]: 100%|██████████| 18/18 [00:15<00:00,  1.18it/s]
Epoch 42/50 - Train Loss: 1.0335, Train Accuracy: 45.57%, Validation Loss: 1.0188, Validation Accuracy: 47.62%
Epoch 43/50 [LP]: 100%|██████████| 157/157 [02:24<00:00,  1.08it/s, loss=1.01] 
Epoch 43/50 [Validating]: 100%|██████████| 18/18 [00:16<00:00,  1.09it/s]
Epoch 43/50 - Train Loss: 1.0359, Train Accuracy: 45.23%, Validation Loss: 1.0223, Validation Accuracy: 46.96%
Epoch 44/50 [LP]: 100%|██████████| 157/157 [02:20<00:00,  1.12it/s, loss=1.05]
Epoch 44/50 [Validating]: 100%|██████████| 18/18 [00:15<00:00,  1.18it/s]
Epoch 44/50 - Train Loss: 1.0332, Train Accuracy: 45.56%, Validation Loss: 1.0223, Validation Accuracy: 47.39%
Epoch 45/50 [LP]: 100%|██████████| 157/157 [02:46<00:00,  1.06s/it, loss=1.04]
Epoch 45/50 [Validating]: 100%|██████████| 18/18 [00:17<00:00,  1.03it/s]
Epoch 45/50 - Train Loss: 1.0347, Train Accuracy: 45.13%, Validation Loss: 1.0219, Validation Accuracy: 47.50%
Epoch 46/50 [LP]: 100%|██████████| 157/157 [02:28<00:00,  1.06it/s, loss=1.06]
Epoch 46/50 [Validating]: 100%|██████████| 18/18 [00:15<00:00,  1.18it/s]
Epoch 46/50 - Train Loss: 1.0343, Train Accuracy: 45.21%, Validation Loss: 1.0221, Validation Accuracy: 47.08%
.....
Epoch 49/50 - Train Loss: 1.0311, Train Accuracy: 45.45%, Validation Loss: 1.0247, Validation Accuracy: 46.59%
Epoch 50/50 [LP]: 100%|██████████| 157/157 [02:23<00:00,  1.09it/s, loss=1.03] 
Epoch 50/50 [Validating]: 100%|██████████| 18/18 [00:15<00:00,  1.13it/s]
Epoch 50/50 - Train Loss: 1.0317, Train Accuracy: 45.57%, Validation Loss: 1.0202, Validation Accuracy: 47.56%
```
### Notes
- The model was saved at specific epochs where validation accuracy improved.
- Training and validation performance is logged at each step.
- The logs include per-epoch loss and accuracy for both training and validation sets.


