### Training Results

Linear probing was done for 100 epochs.
Finetuning was done for 150 epochs.
> **Train:Val Split** = 90:10

<details>
  <summary>Click to expand results</summary>

| Epochs | Phase  | Val Acc (%) | Class 0 AUC | Class 1 AUC | Class 2 AUC | Micro Avg AUC | Notes |
|--------|--------|------------|-------------|-------------|-------------|---------------|-------|
| 50     | LP     | 44.52      | 0.66        | 0.67        | 0.54        | 0.63          | Linear Probing |
| 100    | LP     | 47.95      | 0.70        | 0.71        | 0.56        | 0.66          | Linear Probing |
| **150** | **FT** | **85.12**  | **0.93**    | **0.98**    | **0.87**    | **0.93**      | **Fine-tuning** |

</details>




-------

ROC - AUC LP <INITIAL>
![image](https://github.com/user-attachments/assets/4272e09c-080e-401b-abf1-866ee9ec23bf)
ROC - AUC LP <FINAL>
![image](https://github.com/user-attachments/assets/d0fd9aef-c96e-445d-98a0-5f465b165d7c)
ROC - AUC Curve Fine tuning
![image](https://github.com/user-attachments/assets/4da241c4-b25e-4191-a5bb-1b184e2dced9)
