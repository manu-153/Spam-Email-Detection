# 📧 Spam Email Detection using Logistic Regression & TF-IDE

## 🚀 Project Overview

This project focuses on detecting **spam emails** using **Logistic Regression** and **TF-IDF (Term Frequency-Inverse Document Frequency)** vectorization. It uses a labeled dataset of SMS messages and applies machine learning techniques to classify messages as either "Spam" or "Ham" (non-spam).

## 🧠 Key Concepts

* Natural Language Processing (NLP)
* Text Preprocessing
* TF-IDF Vectorization
* Logistic Regression Classification
* Data Visualization
* Model Evaluation Metrics

---

## 📂 Dataset

The dataset is a CSV file (`spam.csv`) which contains the following columns:

* `v1`: Category (spam or ham)
* `v2`: Message text

Unnecessary columns are removed, and the relevant columns are renamed to:

* `Category`: Converted to 0 (spam) and 1 (ham)
* `Message`: The actual message content

---

## 🛠️ Technologies Used

* Python
* Pandas & NumPy
* Scikit-learn
* NLTK (Stopwords)
* Matplotlib & Seaborn (Visualizations)

---

## 📊 Data Visualization

* **Bar Chart**: Distribution of spam vs. ham messages
* **Pie Chart**: Proportion of spam and ham messages
* **Confusion Matrix**: Model performance visualization
* **Top Words**: Most common words in spam messages (excluding stopwords)

---

## 📈 Model Pipeline

1. **Data Preprocessing**

   * Drop unnecessary columns
   * Encode labels (`spam`: 0, `ham`: 1)
   * Handle null values (if any)

2. **Data Splitting**

   * Train-Test split using `train_test_split()`

3. **Vectorization**

   * Text transformed to numerical features using **TF-IDF**

4. **Model Training**

   * Classifier: **Logistic Regression**
   * Evaluated using **accuracy score** and **confusion matrix**

5. **Prediction**

   * Evaluate on training and test data
   * Predict custom messages (example included)

---

## ✅ Model Performance

* **Training Accuracy**: 97%
* **Testing Accuracy**: 96%

> This indicates a well-generalized model with minimal overfitting.

---

## 🔍 Sample Prediction

```python
new_mail = ["Congratulations on your recent achievement! Well done."]
prediction = model.predict(vectorizer.transform(new_mail))
```

Output:

```
Prediction: Ham Mail
```

---

## 📉 Most Frequent Words in Spam

A bar chart showcasing the **top 7 most common words** in spam emails (excluding stopwords) is also included to provide insight into typical spam content.

---

## 📁 File Structure

```
spam_email_classifier/
├── spam.csv                # Dataset file (not included here for license reasons)
├── spam_detector.py        # Main code file (your script)
├── README.md               # Project documentation
```

---

## 📌 Note

* The dataset used should be placed in the path defined in `file_path` (you can modify it accordingly).
* NLTK stopwords are downloaded at runtime using `nltk.download('stopwords')`.

---

## 🤝 Acknowledgements

* Dataset Source: [UCI SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection)
* Inspired by classical NLP spam detection techniques.

