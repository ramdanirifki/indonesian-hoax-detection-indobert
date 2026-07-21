# 📂 Dataset

This repository **does not include the training dataset** to avoid redistributing third-party data. Please download the original dataset directly from its official source.

---

## Original Dataset

The experiments were conducted using the publicly available **Indonesian Fact and Hoax Political News** dataset available on Kaggle.

**Kaggle:**
https://www.kaggle.com/datasets/linkgish/indonesian-fact-and-hoax-political-news

---

## Dataset Construction

The original dataset is distributed as four Microsoft Excel (`.xlsx`) files:

- `dataset_cnn_10k_cleaned.xlsx`
- `dataset_kompas_4k_cleaned.xlsx`
- `dataset_tempo_6k_cleaned.xlsx`
- `dataset_turnbackhoax_10k_cleaned.xlsx`

For this study, the four datasets were integrated into a single dataset. Duplicate records were removed, labels were standardized, and text preprocessing was subsequently performed before model training and evaluation.

---

## Final Dataset Statistics

| Category | Number of Articles |
|----------|-------------------:|
| Fact | 20,945 |
| Hoax | 10,365 |
| **Total** | **31,310** |

---

## Notes

- The dataset is **not redistributed** in this repository.
- The preprocessing pipeline includes text cleaning, duplicate removal, and label normalization.
- The final dataset was split into **80% training**, **10% validation**, and **10% testing** using **stratified sampling** to preserve the class distribution across all subsets.