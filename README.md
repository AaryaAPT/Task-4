# Logistic Regression - Breast Cancer Classification 🧬

This project implements a **binary classification** using **Logistic Regression** to detect whether a tumor is **malignant (M)** or **benign (B)** based on the Breast Cancer Wisconsin dataset.

## 📁 Dataset

- Source: `data.csv` (Breast Cancer Wisconsin Dataset)
- Target column: `diagnosis`
  - Malignant → `1`
  - Benign → `0`
- Unnecessary columns dropped: `id`, `Unnamed: 32`

---

## 🔧 Tools & Libraries Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## ✅ Steps Followed

### 1. Data Preprocessing

- Loaded dataset
- Dropped non-relevant columns
- Encoded target labels (`M` = 1, `B` = 0)
- Standardized the features

### 2. Train-Test Split

- 80% training
- 20% testing

### 3. Model Training

- Used `LogisticRegression()` from `sklearn.linear_model`
- Fit the model on the scaled training data

### 4. Model Evaluation

Metrics used:
- Confusion Matrix
- Precision
- Recall
- ROC-AUC Score
- ROC Curve Plot

### 5. Threshold Tuning

- Evaluated model using default threshold (0.5)
- Also tested a custom threshold (0.3) to examine precision-recall tradeoff

---

## 📊 Sample Output

```
Confusion Matrix:
[[71  1]
 [ 2 40]]
Precision: 0.9756
Recall: 0.9523
ROC-AUC Score: 0.9943
```

---

## 📈 ROC Curve

The ROC curve plots the **True Positive Rate** vs **False Positive Rate** for different threshold values. Area under the curve (AUC) represents the model's performance.
