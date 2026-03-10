# Student Retention & Churn Prediction

This repository contains a predictive analysis notebook for student retention and churn. The goal is to explore the dataset, visualize key relationships, and build models to predict whether a student will churn or be retained.

The dataset includes student demographics, enrollment information, and opportunity data. Using these features, models predict churn status and identify the key factors influencing drop-offs.

---

## Exploration

The notebook starts with a data exploration step. A **correlation heatmap** is used to see how numeric features relate to each other. Missing values and categorical columns are handled, and new features like "days to apply" are calculated from date columns.

---

## Models

Two classification models were trained and evaluated:

- Logistic Regression  
- Random Forest Classifier  

Both models were evaluated using confusion matrices, accuracy, and churn-specific precision metrics.

---

## Results

### Confusion Matrices

**Logistic Regression**

| Actual \ Predicted | 0      | 1      |
|------------------|--------|--------|
| 0                | 156    | 25     |
| 1                | 36     | 77     |

**Random Forest**

| Actual \ Predicted | Retained | Churned |
|------------------|---------|---------|
| Retained         | 178     | 14      |
| Churned          | 22      | 91      |

---

### Accuracy Comparison

| Model             | Accuracy (%) | Complement to 100 (%) |
|------------------|-------------|----------------------|
| Logistic Regression | 79.67      | 20.33                |
| Random Forest      | 88.20      | 11.80                |
| **Average**        | 83.935     | 16.065               |

---

### Model Metrics

| Metric     | Random Forest | Logistic Regression |
|------------|---------------|------------------|
| Accuracy   | 0.882         | 0.7967           |
| Precision (Churn) | 0.87          | 0.7476           |

---

### Key Drivers of Churn

**Feature Importance**

| Feature                   | Importance |
|----------------------------|-----------|
| Country                    | 0.35      |
| Current/Intended Major     | 0.22      |
| Days to Apply              | 0.17      |
| Age                        | 0.15      |
| Opportunity Duration       | 0.06      |
| Opportunity Category       | 0.04      |
| Churn Gender               | 0.03      |

**Logistic Regression Coefficients**

| Feature                   | Coefficient |
|----------------------------|------------|
| Opportunity Duration       | 0.05       |
| Age                        | 0.15       |
| Opportunity Category       | 0.03       |
| Churn Gender               | 0.02       |
| Current/Intended Major     | 0.22       |
| Days to Apply              | 0.17       |
| Country                    | 0.35       |

---

## Visuals

Correlation heatmap, confusion matrices, accuracy comparison, and feature importance charts:

**Heatmap**
<img width="1154" height="658" alt="HEATMAP" src="https://github.com/user-attachments/assets/86542b54-2cb2-4bd8-b1ab-1668e121838d" />
**Logistic Regression Confusion Matrix**
<img width="1071" height="636" alt="Logistic Regression" src="https://github.com/user-attachments/assets/665f4cb5-38d0-49c3-89d8-6ad44c7e5987" />


**Random Forest Confusion Matrix**
<img width="1126" height="621" alt="Random Forest" src="https://github.com/user-attachments/assets/0a85071f-c148-4668-ae54-b0d7e2166fd5" />


**Accuracy**
<img width="1214" height="612" alt="Accuracy vs Error" src="https://github.com/user-attachments/assets/104a14b5-5829-47b5-ace8-da2a310c8182" />


**Model Comparison**
<img width="1207" height="625" alt="comparison" src="https://github.com/user-attachments/assets/6d942785-4256-403e-8a6d-50c03f7fdc27" />


**Logistic Regression: Feature Impact**
<img width="937" height="622" alt="Featre impact" src="https://github.com/user-attachments/assets/8d259c68-38a3-4b30-979e-8e520038c55a" />


**Key Drivers of Churn**
<img width="1145" height="653" alt="keydriver" src="https://github.com/user-attachments/assets/a69a78c9-0ff1-40f6-bfe5-82a3ea203206" />



---

## Files

- student_churn_analysis.ipynb  
- README.md

---

## Author
Maryam Zafar

## GitHub
https://github.com/mimizfr
