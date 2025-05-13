# 💳 Credit Card Fraud Detection

## 🧾 Project Overview

With increasing online financial transactions, fraud detection has become a crucial area of interest for financial institutions. This project focuses on detecting fraudulent credit card transactions using machine learning. It builds and evaluates various classification models to classify transactions as fraudulent or legitimate with high precision and recall, especially considering the imbalanced nature of real-world fraud datasets.

---

## 🎯 Problem Statement

Financial fraud results in billions of dollars in losses annually. Detecting fraudulent credit card transactions early helps in reducing these losses. However, fraud detection is challenging due to:

- Highly imbalanced datasets (fraudulent transactions are rare)
- Need for fast, real-time predictions
- Avoiding too many false positives (which inconvenience users)

This project addresses these challenges by building an end-to-end machine learning pipeline that includes preprocessing, handling class imbalance, and comparing different ML algorithms.

---

## 📁 Dataset Information

- **Source**: [Credit Card Transactions Dataset](https://raw.githubusercontent.com/ArchanaInsights/Datasets/refs/heads/main/credit_card_transactions.csv)
- **Size**: ~30,000 records
- **Target Column**: `Is_Fraudulent` (Yes/No)
- **Key Features**:
  - `Transaction_ID`, `Transaction_Amount`
  - `Merchant_Category`, `Card_Type`, `Use_Chip`, `Online_Order`
  - `Location`, `Time`, `Device_Type`, `Entry_Mode`

---

## 📊 Exploratory Data Analysis (EDA)

- Analyzed fraud vs. non-fraud distribution
- Explored transaction amounts, regions, and merchant categories
- Found trends such as higher fraud in online orders and specific merchant types
- Identified that fraud often involves high transaction amounts or certain card types

---

## 🧹 Data Preprocessing

- **Missing Values**: Imputed using KNN Imputer
- **Outlier Handling**: Removed extreme transaction amounts
- **Categorical Encoding**:
  - Label Encoding for binary columns
  - One-Hot Encoding for categorical features with multiple classes
- **Feature Scaling**: Applied StandardScaler on continuous features
- **Duplicates**: Removed duplicates based on `Transaction_ID`

---

## ⚖️ Handling Class Imbalance

- Fraudulent transactions make up a very small fraction of the dataset
- Instead of synthetic oversampling, focused on:
  - Stratified train-test split
  - Emphasizing **recall** and **F1-score** for the fraud class
  - Selecting models with balanced performance

---

## 🧠 Model Building & Evaluation

### ML Algorithms Applied:
- Logistic Regression
- Random Forest Classifier ✅ (Best performing)
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Naive Bayes

### Evaluation Metrics:
- Accuracy
- Precision
- Recall (key focus)
- F1-score
- Confusion Matrix

**✅ Logistic Regression Results:**
- Strong recall for fraud detection
- Balanced precision/recall
- Lowest false negatives among all tested models

**Best Model Performance (Random Forest Classifier):**
- High recall and precision for the minority fraud class
- Balanced accuracy for both classes

## 🛠️ Technologies Used

- **Language**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Tools**: Jupyter Notebook, GitHub
- **ML Techniques**: Supervised classification, encoding, scaling, performance evaluation

## 📊 Results
- Achieved strong fraud detection accuracy using Random Forest
- Built a scalable ML pipeline for fraud detection
- Demonstrated importance of feature scaling, encoding, and class balancing

## 📌 Conclusion
This project demonstrates how machine learning can be used to enhance credit card fraud detection. It offers a practical framework that can be extended for real-time fraud prevention systems.

