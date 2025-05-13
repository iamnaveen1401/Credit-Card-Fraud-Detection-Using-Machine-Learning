# 💳 Credit Card Fraud Detection

## 🧾 Project Overview

With the rise of online payments, detecting fraudulent credit card transactions has become a critical challenge. This project aims to develop a robust machine learning model that accurately identifies fraudulent transactions in real-time. The model helps financial institutions minimize financial losses and improve transaction security while maintaining a low false-positive rate.

## 📁 Dataset

- **Source**: [Credit Card Transactions Dataset](https://raw.githubusercontent.com/ArchanaInsights/Datasets/refs/heads/main/credit_card_transactions.csv)
- **Attributes**:
  - `Transaction_ID`, `Card_Type`, `Merchant_Category`, `Transaction_Amount`, `Location`, `Region`, etc.
  - `Is_Fraudulent`: Target variable indicating fraud status (Yes/No)

## 🔍 Key Steps

### 1. Exploratory Data Analysis (EDA)
- Analyzed categorical features like card type, merchant category, and device type
- Visualized transaction patterns for fraud vs. non-fraud

### 2. Data Preprocessing
- Handled missing values using KNNImputer and other imputation techniques
- Removed outliers and transformed skewed features
- Scaled numerical features for consistency

### 3. Feature Engineering & Selection
- Encoded categorical features using one-hot and label encoding
- Selected important features for model input

### 4. Model Building & Evaluation
- Trained multiple classification models:
  - Logistic Regression
  - Random Forest
  - Support Vector Machine (SVM)
  - K-Nearest Neighbors (KNN)
  - Naive Bayes
- Evaluated models using:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
  - Confusion Matrix

## 🛠️ Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

## 📊 Results
- Achieved high performance with optimal model based on F1-score
- Successfully reduced false positives while maintaining high fraud detection rate

## 📌 Conclusion
This project demonstrates how machine learning can be used to enhance credit card fraud detection. It offers a practical framework that can be extended for real-time fraud prevention systems.
