# 💳 Credit Card Fraud Detection - Capstone Project

## 📌 Problem Statement

The objective of this project is to **predict fraudulent credit card transactions** using machine learning models.

We analyze **customer-level transaction data** obtained from a research collaboration between **Worldline** and the **Machine Learning Group**. The dataset contains **284,807 transactions**, of which only **492 are fraudulent** — highlighting a **highly imbalanced classification problem**.

---

## 🧠 Business Problem Overview

For banks and financial institutions, **retaining profitable customers** is a primary objective. However, **banking fraud** threatens this goal significantly.

According to a **Nilson report**, banking fraud was estimated to reach **$30 billion globally by 2020**. With the growth of digital payment systems, fraudulent transactions are evolving in both **number and method**.

**Machine learning** helps in:
- Automating fraud detection
- Reducing chargebacks and fees
- Avoiding denial of legitimate transactions
- Minimizing manual review efforts

Thus, implementing fraud detection using machine learning is **crucial** in today's banking systems.

---

## 🚨 Understanding & Defining Fraud

**Credit card fraud** is any unauthorized or deceptive activity intended to gain access to financial information for personal gain. Common fraud types include:

- 🔁 Skimming (duplication of card data)
- 🧾 Alteration of genuine cards
- 🏷️ Counterfeit card creation
- 🧳 Lost/stolen cards
- ☎️ Fraudulent telemarketing

---

## 🧾 Data Dictionary

The dataset (available on [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)) contains **credit card transactions by European cardholders** over **two days** in September 2013.

| Feature        | Description |
|----------------|-------------|
| `Time`         | Seconds elapsed since the first transaction |
| `Amount`       | Transaction amount |
| `V1` to `V28`  | Principal components from PCA (due to confidentiality) |
| `Class`        | Target label (1: Fraud, 0: Non-Fraud) |

> ⚠️ **Note:** Only **0.172%** of transactions are fraudulent — special care is needed to handle the **class imbalance**.

---

## 🔁 Project Pipeline

1. ### 📊 Data Understanding
   - Load and inspect the dataset
   - Understand distributions and relevance of each feature

2. ### 🔎 Exploratory Data Analysis (EDA)
   - Perform univariate and bivariate analysis
   - Check for **skewness** and **transform** features if needed
   - Z-scaling is not required (Gaussian features already)

3. ### ✂️ Train/Test Split
   - Use **Stratified K-Fold Cross Validation** to ensure balanced class distribution in folds

4. ### 🤖 Model Building & Hyperparameter Tuning
   - Try various ML algorithms
   - Apply **sampling techniques** (e.g., SMOTE, undersampling)
   - Tune parameters for best performance

5. ### 📈 Model Evaluation
   - Use appropriate metrics:
     - **Precision**
     - **Recall**
     - **F1-Score**
     - **ROC-AUC**
   - Emphasis on **minimizing false negatives** (i.e., missed frauds)

---

## 🧪 Technologies Used

- Python (Pandas, NumPy, Scikit-learn, Imbalanced-learn)
- Jupyter Notebook
- Matplotlib / Seaborn (for visualization)

---

## 📂 Dataset Source

Kaggle: [Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

---

## 📌 Conclusion

By building robust models and addressing the class imbalance effectively, **credit card fraud** can be identified accurately and proactively — reducing loss and improving customer trust.
