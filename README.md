# Imbalanced Data Handling and Model Building

This project demonstrates techniques for handling **imbalanced datasets** in classification problems, specifically applied to **credit card transaction data**. Alongside the code, explanations of the methods are provided for better understanding.

**Data Source:** [Credit Card Transactions Dataset - Kaggle](https://www.kaggle.com/datasets/priyamchoksi/credit-card-transactions-dataset)

---

## Project Overview

In many real-world datasets, like credit card transactions, the classes are highly imbalanced. For example, fraudulent transactions are much rarer than legitimate ones. Handling such imbalance is critical to ensure accurate model performance.

This project explores three common methods for addressing class imbalance:

---

## Method 1: Random Undersampling

**Description:**  
Random Undersampling reduces the number of observations in the majority class until a more balanced class distribution is achieved.

**Advantages:**  
- Simple and fast to implement  
- Computationally efficient  

**Drawbacks:**  
- May discard useful information from the majority class  
- Can reduce the model’s ability to generalize  

---

## Method 2: Random Oversampling

**Description:**  
Random Oversampling duplicates samples from the minority class until the classes are balanced.

**Advantages:**  
- Preserves informative patterns from the minority class  
- Avoids losing majority class data  

**Drawbacks:**  
- May lead to overfitting due to duplication of data  

---

## Method 3: SMOTE (Synthetic Minority Over-sampling Technique)

**Description:**  
SMOTE generates **synthetic samples** for the minority class by interpolating between existing samples and their nearest neighbors, rather than duplicating them.  

**Advantages:**  
- Reduces the risk of overfitting compared to Random Oversampling  
- Maintains the original data distribution and generates realistic synthetic samples  

**How it Works:**  
- **S** – Synthetic  
- **M** – Minority  
- **O** – Over-sampling  
- **T** – Technique  

SMOTE effectively balances the dataset while improving model generalization.

---

## Conclusion

By applying these methods, we can better handle imbalanced datasets, improving the performance and reliability of classification models in critical tasks like fraud detection.
