#  Spam Email Detection — Logistic Regression

##  Project Overview 

---

##  Key Concepts
- Natural Language Processing (NLP)  
- Text preprocessing (tokenization, stopword removal)  
- TF‑IDF vectorization  
- Logistic Regression classification  
- Model evaluation (accuracy, confusion matrix)  
- Data visualization

---

##  project Dataset
- Source file: `spam.csv`  
- Original columns:  
  - `v1`: category (spam or ham)  
  - `v2`: message text

- Processed/renamed columns used in this project:  
  - `Category`: encoded as 0 = spam, 1 = ham  
  - `Message`: raw message text

Unnecessary columns are removed and null values are handled during preprocessing.

---

## Tech Stack
- Python  
- pandas, NumPy  
- scikit-learn  
- NLTK (stopwords)  
- Matplotlib, Seaborn

---

## Visualizations
- Bar chart: distribution of spam vs. ham messages  
- Pie chart: proportion of spam and ham  
- Confusion matrix: classification performance  
- Bar chart: top 7 most frequent words in spam (stopwords excluded)

---

## Model Pipeline
1. Data preprocessing  
   - Drop irrelevant columns  
   - Encode labels (spam → 0, ham → 1)  
   - Handle missing values  
   - Basic text cleaning and stopword removal (NLTK)

2. Train / test split using `train_test_split()`.

3. Vectorization  
   - Convert text to numerical features with TF‑IDF.

4. Model training  
   - Classifier: Logistic Regression  
   - Evaluate with accuracy and confusion matrix

5. Prediction  
   - Evaluate on train and test sets  
   - Support example/custom message prediction

---

## Model Performance
- Training accuracy: 97%  
- Testing accuracy: 96%

This suggests good generalization with minimal overfitting on the provided dataset.

---

## Example: Predicting a New Message
```python
# assuming `vectorizer` and `model` are already trained
new_mail = ["Congratulations on your recent achievement! Well done."]
pred = model.predict(vectorizer.transform(new_mail))
label = "Ham" if pred[0] == 1 else "Spam"
print(f"Prediction: {label} Mail")

Top Words in Spam
A visualization is included that highlights the top 7 most common words in spam messages (after removing stopwords) to give quick insight into typical spam content.

Project Structure
spam_email_classifier/
├── spam.csv                # Dataset (not included in this repo)
├── spam_detector.py        # Main script
├── README.md               # Project documentation


Notes

* Place the dataset at the path specified by the file_path variable (modify as needed).
* NLTK stopwords are downloaded at runtime (nltk.download('stopwords')).
* Install required packages (example):
pip install pandas numpy scikit-learn nltk matplotlib seaborn
