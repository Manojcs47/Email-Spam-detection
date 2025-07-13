# Email Spam Detection Using Logistic Regression

## 1. Project Overview
This project implements a machine learning model to classify emails as either "spam" or "ham" (not spam). The goal is to build an effective classifier using Logistic Regression and evaluate its performance on a real-world dataset. This is a classic binary classification task.

***

## 2. Dataset
* **Source:** The dataset used is `mail_data.csv`.
* **Content:** The dataset contains two primary columns: `Category`, which labels the email as spam or ham, and `Message`, which contains the raw text of the email.

***

## 3. Methodology
* **Data Preprocessing:** The categorical labels were encoded into numerical values (spam: 0, ham: 1) for model compatibility. 
* **Feature Extraction:** Text data from the email messages was converted into numerical feature vectors using `TfidfVectorizer`. This technique reflects the importance of a word in an email relative to the entire dataset.
* **Model Training:** A **Logistic Regression** model from the `scikit-learn` library was trained on the processed training data.
* **Evaluation:** The model's performance was evaluated using accuracy, precision, recall, F1-score, and ROC-AUC.

***

## 4. Preliminary Results
The model demonstrated high effectiveness in classifying emails on the unseen test data. The key performance metrics are summarized below.

| Metric | Score |
| :--- | :--- |
| **Accuracy** | 96.7% |
| **Precision** | 96.5% |
| **Recall** | 99.7% |
| **F1-Score** | 98.1% |
| **ROC-AUC** | 0.992 |

The high scores, particularly for precision and recall, indicate that the model is very effective at both correctly identifying legitimate emails and filtering out spam.
