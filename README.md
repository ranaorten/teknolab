# TeknoLAB — Introduction to Machine Learning

## Ödevler

| # | İçerik |
|---|--------|
| **Ödev 1** | Sunum kırmızı işaretli konular: Confusion Matrix, Precision & Recall, F1 Score, ROC-AUC, Regularization hyperparameter |
| **Ödev 2** | StatQuest video listesi (ML Day 1 tekrar + Day 2 hazırlık) |
| **Ödev 3** | Programlama ödevi → `homework1.ipynb` |

## Ödev 3 — Taming the Imbalanced Dataset

**Dataset:** German Credit Risk (`data/german_credit.csv`)  
**Hedef:** Dengesiz sınıf probleminde Logistic Regression ile Risk sınıfı (class 1) için recall ve F1-score'u iyileştirmek.

### Teknikler ve sonuçlar

| Technique | Accuracy | Precision (1) | Recall (1) | F1 (1) |
|-----------|----------|---------------|------------|--------|
| Baseline | 0.735 | 0.600 | 0.350 | 0.442 |
| Class weights (balanced) | 0.750 | 0.571 | **0.667** | **0.615** |
| Threshold moving (thr=0.3) | 0.735 | 0.551 | 0.633 | 0.589 |
| Random oversampling | 0.755 | 0.585 | 0.633 | 0.608 |
| SMOTE (optional) | 0.730 | 0.544 | 0.617 | 0.578 |

### Çalıştırmak için

```bash
pip install scikit-learn imbalanced-learn pandas jupyter
jupyter notebook homework1.ipynb
```
