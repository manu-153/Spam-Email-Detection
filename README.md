# 📧 Spam Email Detection Using Logistic Regression and TF-IDF

## 📝 Project Overview

This project focuses on building a **spam email classifier** using **Logistic Regression** and **TF-IDF (Term Frequency–Inverse Document Frequency)** for feature extraction. The dataset consists of SMS messages labeled as **spam** or **ham (non-spam)**. The goal is to develop a robust model that can accurately detect and filter out spam messages.

---

## 🔍 Key Features

* **📂 Data Preprocessing**

  * Handles missing values
  * Renames columns for clarity
  * Converts categorical labels (spam/ham) into numerical format (1/0)

* **🔡 Feature Extraction**

  * Uses **TF-IDF Vectorizer** to transform text into numerical features for model consumption

* **🤖 Model Training**

  * Applies **Logistic Regression** for binary classification (spam vs. ham)

* **📊 Model Evaluation**

  * Evaluates model using:

    * Accuracy Score
    * Confusion Matrix
    * Visualization techniques for better interpretability

---

## 📈 Visualizations

The project includes several visualizations for understanding the data distribution and evaluating the model’s performance:

### 1. 📊 Distribution of Emails

Visual representation of class balance in the dataset:

* **Bar Plot**: Shows count of spam vs. ham messages
* **Pie Chart**: Displays proportion (%) of spam vs. ham messages

### 2. 🔁 Confusion Matrix

Illustrates the classifier's performance:

* **True Positives (TP)**: Spam correctly predicted as spam
* **True Negatives (TN)**: Ham correctly predicted as ham
* **False Positives (FP)**: Ham misclassified as spam
* **False Negatives (FN)**: Spam misclassified as ham

### 3. 🧞 Top Words in Spam Emails

* **Bar Chart** displaying the most common and frequent words found in spam messages
* Helps in uncovering recurring keywords typical of spam patterns

---

## 📂 Technologies Used

* Python 🐍
* Pandas, NumPy – Data Manipulation
* Scikit-learn – Model Building and Evaluation
* Matplotlib, Seaborn – Visualization
* TF-IDF Vectorizer – Feature Engineering
* Jupyter Notebook – Development Environment

---

## ✅ Final Thoughts

This project demonstrates how classical machine learning models like Logistic Regression, when combined with smart text feature engineering (TF-IDF), can perform well for binary classification tasks such as spam detection. It's a great entry point for NLP tasks and spam filtering systems.


