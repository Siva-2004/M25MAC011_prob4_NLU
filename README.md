# Sports vs Politics Text Classification

## Overview
Implementation of a supervised machine learning system to classify text documents into two categories: **Sports** and **Politics**. The goal is to compare traditional machine learning techniques using different feature representations and analyze their performance on a real-world text dataset.

---

## Dataset
The dataset consists of news articles collected from publicly available sources.  
Only two categories are used:

- **Sports**
- **Politics**

### Dataset Source
- BBC News Dataset (filtered to Sports and Politics categories)
- DeepTweets

## Text Preprocessing
The following preprocessing steps were applied:

- Converted text to lowercase
- Removed URLs
- Removed user mentions and hashtags
- Removed non-alphanumeric characters
- No stemming or lemmatization was applied

---

## Feature Extraction
- **TF-IDF (Term Frequency–Inverse Document Frequency)**

TF-IDF representation was applied for this task.

---

## Machine Learning Models
Three machine learning models were implemented and compared:

1. **Naive Bayes**
2. **Logistic Regression**
3. **Support Vector Machine (SVM)**

All models were trained using the same train-test split to ensure a fair comparison.

---

## Evaluation
- Dataset split: 80% training, 20% testing
- Primary evaluation metric: **Accuracy**

### Results Summary

| Model | Accuracy |
|------|---------|
| Naive Bayes | 94.47% |
| Logistic Regression | 93.21% |
| SVM | 94.82% |

SVM achieved the best overall performance when combined with TF-IDF features.

---

## Limitations
- The system relies only on TF-IDF features and does not capture semantic meaning.
- No stemming or lemmatization is used, resulting in separate features for word variants.
- Contextual and long-range dependencies are not captured.
- The model is limited to binary classification (Sports vs Politics).

---

## Conclusion
This project demonstrates that traditional machine learning techniques can effectively classify text documents when combined with appropriate feature representations. Among the evaluated models, SVM with TF-IDF features performed best. Future work may explore deep learning models and contextual embeddings for improved performance.

