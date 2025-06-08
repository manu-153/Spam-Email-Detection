# Spam Email Detection Using Logistic Regression and TF-IDF

## Project Overview

This project aims to classify email messages as spam or ham (non-spam) using a Logistic Regression model and Term Frequency-Inverse Document Frequency (TF-IDF) for feature extraction. The dataset used is a collection of SMS messages, and the objective is to build an effective classifier for spam detection.

### Key Features

- **Data Preprocessing**: Handles missing values, renames columns, and converts categorical labels to numerical values.
- **Feature Extraction**: Utilizes TF-IDF to convert text data into numerical features.
- **Model Training**: Implements Logistic Regression for classification.
- **Model Evaluation**: Evaluates performance using accuracy, confusion matrix, and visualizations.
## Visualizations

The project includes several visualizations to help understand the data and evaluate the performance of the spam email detection model:

1. **Distribution of Emails**

   This visualization shows the distribution of spam and ham emails. It includes:
   - **Bar Plot**: Illustrates the count of spam vs. ham emails.
   - **Pie Chart**: Represents the percentage of spam vs. ham emails.

2. **Confusion Matrix**

   The confusion matrix visualizes the performance of the Logistic Regression model in classifying emails as spam or ham. It provides insights into:
   - **True Positives**: Correctly identified spam emails.
   - **True Negatives**: Correctly identified ham emails.
   - **False Positives**: Ham emails incorrectly identified as spam.
   - **False Negatives**: Spam emails incorrectly identified as ham.

3. **Top Words in Spam Emails**

   This bar chart displays the most frequent words found in spam emails. It helps in identifying common patterns or keywords that are typical in spam messages.


