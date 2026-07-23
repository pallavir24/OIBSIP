# Task 1: Iris Flower Classification 🌸

## 📌 Project Overview
This project focuses on building a Machine Learning classification model to identify the species of an Iris flower (**Setosa**, **Versicolor**, or **Virginica**) based on its physical measurements:
* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

---

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** `scikit-learn`, `pandas`, `numpy`, `matplotlib`, `seaborn`
* **Environment:** Jupyter Notebook

---

## 📋 Feature Checklist & Implementation

- [x] **Data Loading:** Loaded directly via `sklearn.datasets.load_iris()`
- [x] **Exploratory Data Analysis (EDA):**
  - Verified shape, data types, and checked for missing values (`df.isnull().sum()`)
  - Calculated descriptive statistics (`df.describe()`)
- [x] **Data Visualizations:**
  - `sns.pairplot` to visualize feature distributions across species
  - Box plots to inspect feature spreads and identify discriminative attributes
- [x] **Model Training & Evaluation:**
  - Performed an 80/20 train/test split using `train_test_split`
  - Trained multiple classifiers (Logistic Regression, K-Nearest Neighbors, Random Forest)
  - Evaluated using **Accuracy Score**, **Confusion Matrix**, and **Classification Report** (Precision, Recall, F1-Score)
- [x] **Model Selection:** Selected the best-performing model based on cross-validation and test performance metrics.

---
