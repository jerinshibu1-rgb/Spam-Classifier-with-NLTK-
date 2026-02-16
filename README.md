#  Spam Classifier using NLTK

A Machine Learning–based **Spam Detection System** that classifies messages as **Spam** or **Ham (Not Spam)** using **Natural Language Processing (NLP)** techniques and **NLTK**.  
This project demonstrates the complete NLP pipeline from text preprocessing to model evaluation.

---

##  Project Overview

Spam messages pose security and usability risks in email and messaging platforms.  
This project builds an automated spam classifier that:

- Preprocesses raw text using NLP techniques
- Converts text into numerical features using TF-IDF
- Trains a machine learning model to detect spam messages
- Evaluates performance using standard classification metrics

---

##  Technologies Used

- **Python**
- **NLTK** – Text preprocessing
- **Pandas & NumPy** – Data manipulation
- **Scikit-learn** – Feature extraction, modeling, evaluation
- **Jupyter Notebook**

---

##  Dataset Description

The dataset consists of labeled text messages:

| Column | Description |
|------|------------|
| `message` | SMS / email text |
| `label` | `spam` or `ham` |

**Key characteristics:**
- Unstructured text data
- Class imbalance (ham > spam)
- Real-world noisy text (symbols, links, slang)

---

##  NLP Preprocessing Steps

The following preprocessing steps are applied using **NLTK**:

1. Convert text to lowercase  
2. Tokenization  
3. Remove punctuation and numbers  
4. Remove stopwords  
5. Apply stemming / lemmatization  

These steps transform raw text into clean, meaningful tokens for modeling.

---

##  Feature Engineering

- **Bag of Words (BoW)**
- **TF-IDF (Term Frequency–Inverse Document Frequency)**  *(final choice)*

TF-IDF performed better by emphasizing important words commonly found in spam messages.

---

##  Model Building

The following algorithms were experimented with:

- Multinomial Naive Bayes  *(final model)*
- Logistic Regression
- Support Vector Machine (optional)

**Why Naive Bayes?**
- Optimized for text classification
- Fast and memory-efficient
- Works well with sparse TF-IDF features

---

##  Model Evaluation

Evaluation metrics used:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

###  Final Performance
- **Accuracy:** ~97–98%
- **High precision and recall for spam class**
- Minimal false positives (ham incorrectly marked as spam)

---

##  Business Impact

-  Automatically filters spam messages  
-  Enables real-time message screening  
-  Improves user safety by blocking phishing and scam messages  
-  Reduces manual moderation and operational costs  

---
