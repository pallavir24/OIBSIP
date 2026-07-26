# Task 4: Email Spam Detection with Machine Learning

## 📌 Project Overview
This project focuses on building a **Natural Language Processing (NLP)** binary classification pipeline to accurately distinguish spam messages/emails from legitimate ("ham") ones. Using Python, TF-IDF vectorization, and machine learning algorithms (Multinomial Naive Bayes and Logistic Regression/SVM), the goal is to build an efficient, scalable text classification workflow.

---

## 🛠️ Tech Stack & Dependencies
* **Programming Language:** Python 3.x
* **Environment:** Jupyter Notebook / Google Colab
* **Libraries:**
  * Data Manipulation: `pandas`, `numpy`
  * NLP & Preprocessing: `nltk`, `re` (Regular Expressions)
  * Feature Extraction & ML Models: `scikit-learn`
  * Data Visualization: `matplotlib`, `seaborn`, `wordcloud`

---

## 📁 Dataset
* **Source:** [UCI Machine Learning Repository / Kaggle - SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection)
* **Structure:** Contains raw text messages labeled as either `ham` (legitimate) or `spam`.

---

## 🚀 Key Steps & Implementation Details

### 1. Data Loading & Class Distribution Analysis
* Loaded the raw text dataset into Pandas.
* Analyzed class distribution by computing exact counts and percentage shares of `spam` vs. `ham` messages.

### 2. Text Preprocessing Pipeline
To clean unstructured text data before feature extraction, the following preprocessing steps were applied:
* **Lowercasing:** Converting all text to lowercase.
* **Noise & Punctuation Removal:** Stripping special characters and numbers using regular expressions (`re`).
* **Stopword Removal:** Eliminating non-informative words using NLTK's English stopword list.
* **Stemming / Lemmatization:** Reducing words to their root forms (e.g., using `PorterStemmer` / `WordNetLemmatizer`).

### 3. Feature Extraction (TF-IDF Vectorizer)
Text data was converted into numerical vectors using `TfidfVectorizer`.

> **What is TF-IDF?**  
> **TF-IDF (Term Frequency - Inverse Document Frequency)** measures the relative importance of a word within a specific document compared to a whole corpus.
> * **Term Frequency (TF):** Measures how frequently a term occurs in a given text.
> * **Inverse Document Frequency (IDF):** Penalizes common words across all documents (like "the", "is", "at") and emphasizes domain-specific, informative terms (like "free", "win", "prize").

### 4. Model Training & Evaluation
* **Train/Test Split:** Split the dataset (e.g., 80% training / 20% testing) with stratification.
* **Classifiers Trained:**
  1. **Multinomial Naive Bayes** (Industry standard for text baseline classification)
  2. **Logistic Regression / SVM** (Alternative robust classifier)
* **Performance Metrics:** Evaluated models using Accuracy, Precision, Recall, F1-Score, and Confusion Matrix plots.

---

## 💬 Discussion: Why Recall Matters in Spam Detection

> **Why is Recall particularly important (and how do we balance it with Precision)?**
> * **False Positives (FP):** Marking a legitimate email as *spam* (e.g., a crucial job offer or invoice goes to the spam folder).
> * **False Negatives (FN):** Marking a spam email as *ham* (a spam message lands in the primary inbox).
>
> While **Recall** for the *Spam* class measures how effectively we catch spam messages, **Precision** for the *Spam* class is critical because a **False Positive** (misclassifying crucial legimitate emails as spam) is far more damaging to the user than occasionally letting a spam email slip into the inbox. Thus, tuning models to maximize **Precision/F1-Score** while maintaining high **Recall** is essential in real-world deployment.

---

## 📊 Visualizations & Outputs
* **Class Distribution Bar Chart**
* **Confusion Matrix Heatmaps** for both classifiers
* **WordClouds:**
  * **Spam WordCloud:** Highlights top spam indicators (e.g., *free, win, claim, urgent, call*).
  * **Ham WordCloud:** Highlights everyday communication words (e.g., *go, come, home, ok, call*).

---

## 🗂️ Project Structure
```text
.
├── data/
│   └── spam.csv                  # Dataset file
├── notebooks/
│   └── Spam_Detection.ipynb      # Clean, fully commented Jupyter Notebook
├── README.md                     # Project documentation

