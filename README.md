# 🩺 Stroke Prediction with Imbalanced Data Handling

## 📌 Overview
This project predicts **stroke occurrence** using healthcare data from Kaggle.  
The focus is on **data cleaning, preprocessing, model evaluation, and handling class imbalance**—skills relevant to Data Processing & Analytics (DPA) roles.

Dataset: [Stroke Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)



## ⚡ Workflow

### 1. Data Preprocessing
- Dropped irrelevant column (`id`)
- Filled missing `bmi` values with median
- One-hot encoded categorical variables
- Standardized features using **StandardScaler**

### 2. Exploratory Data Analysis (EDA)
- Checked missing values
- Visualized correlations with a heatmap
- Analyzed class distribution:
  - Stroke cases: ~5%  
  - Non-stroke cases: ~95%

### 3. Modeling
Models used:
- **Logistic Regression**
- **Random Forest**

### 4. Imbalance Handling
- Applied **SMOTE (Synthetic Minority Oversampling Technique)** to balance classes

### 5. Evaluation
Metrics used:
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix


## 📊 Results

### Before Balancing
- Accuracy ≈ 95%  
- Recall for stroke patients ≈ 0–2%  
- Models biased toward predicting **non-stroke**

### After Balancing (SMOTE)
- **Logistic Regression:**
  - Recall for stroke patients improved from 0.02 → 0.80
  - Accuracy dropped to ~75% (expected tradeoff)
- **Random Forest:**
  - Slight improvement in recall (~0.12)
  - Accuracy stayed high (~91%)



## 📝 Key Insights
1. Real-world healthcare data is often **imbalanced**, making raw accuracy misleading.  
2. **Balancing methods (SMOTE)** significantly improve minority class detection.  
3. Logistic Regression provides interpretability (important in healthcare).  
4. Random Forest offers higher accuracy but less recall improvement.  
5. Demonstrates the trade-off between **accuracy, precision, and recall**.  

---
