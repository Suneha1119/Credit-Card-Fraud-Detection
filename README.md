# 💳 Credit Card Fraud Detection - Capstone Project

## 📌 Problem Statement
The problem statement chosen for this project is to predict fraudulent credit card transactions with the help of machine learning models.
In this project, we will analyse customer-level data which has been collected and analysed during a research collaboration of Worldline and the Machine Learning Group.
The dataset is taken from the Kaggle website and it has a total of 2,84,807 transactions, out of which 492 are fraudulent. Since the dataset is highly imbalanced, so it needs to be handled before model building.

---

## 🧠 Business Problem Overview
For many banks, retaining high profitable customers is the number one business goal. Banking fraud, however, poses a significant threat to this goal for different banks. In terms of substantial financial losses, trust and credibility, this is a concerning issue to both banks and customers alike.
It has been estimated by Nilson report that by 2020 the banking frauds would account to $30 billion worldwide. With the rise in digital payment channels, the number of fraudulent transactions is also increasing with new and different ways.
In the banking industry, credit card fraud detection using machine learning is not just a trend but a necessity for them to put proactive monitoring and fraud prevention mechanisms in place. Machine learning is helping these institutions to reduce time-consuming manual reviews, costly chargebacks and fees, and denials of legitimate transactions.

---

## 🚨 Understanding & Defining Fraud

Credit card fraud is any dishonest act and behaviour to obtain information without the proper authorization from the account holder for financial gain. Among different ways of frauds, Skimming is the most common one, which is the way of duplicating of information located on the magnetic strip of the card. Apart from this, the other ways are:
⦁	Manipulation/alteration of genuine cards
⦁	Creation of counterfeit cards
⦁	Stolen/lost credit cards
⦁	Fraudulent telemarketing

---

## 🧾 Data Dictionary

The dataset can be download using this link
The data set includes credit card transactions made by European cardholders over a period of two days in September 2013. Out of a total of 2,84,807 transactions, 492 were fraudulent. This data set is highly unbalanced, with the positive class (frauds) accounting for 0.172% of the total transactions. The data set has also been modified with Principal Component Analysis (PCA) to maintain confidentiality. Apart from ‘time’ and ‘amount’, all the other features (V1, V2, V3, up to V28) are the principal components obtained using PCA. The feature 'time' contains the seconds elapsed between the first transaction in the data set and the subsequent transactions. The feature 'amount' is the transaction amount. The feature 'class' represents class labelling, and it takes the value 1 in cases of fraud and 0 in others.

---

## 🔁 Project Pipeline

1. ### 📊 Data Understanding
  Here, we need to load the data and understand the features present in it. This would help us choose the features that we will need for your final model.

2. ### 🔎 Exploratory Data Analysis (EDA)
 Normally, in this step, we need to perform univariate and bivariate analyses of the data, followed by feature transformations, if necessary. For the current data set, because Gaussian variables are used, we do not need to perform Z-scaling. However, you can check if    there is any skewness in the data and try to mitigate it, as it might cause problems during the model-building phase.

3. ### ✂️ Train/Test Split
  Now we are familiar with the train/test split, which we can perform in order to check the performance of our models with unseen data. Here, for validation, we can use the k-fold cross-validation method. We need to choose an appropriate k value so that the minority class is correctly represented in the test folds.

4. ### 🤖 Model Building & Hyperparameter Tuning
   This is the final step at which we can try different models and fine-tune their hyperparameters until we get the desired level of performance on the given dataset. We should try and see if we get a better model by the various sampling techniques.

5. ### 📈 Model Evaluation
  We need to evaluate the models using appropriate evaluation metrics. Note that since the data is imbalanced it is is more important to identify which are fraudulent transactions accurately than the non-fraudulent. We need to choose an appropriate evaluation metric      which reflects this business goal.

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
