# Car Price Prediction with Machine Learning 🚗

A machine learning project designed to predict the selling price of used cars based on key features such as brand, vehicle age, mileage, fuel type, transmission, and seller type.

---

## 📌 Project Overview
The objective of this project is to build and evaluate regression models to accurately forecast used car prices. By analyzing historical vehicle data, the model identifies key factors influencing vehicle valuation, helping buyers and sellers make informed decisions.

This project was completed as part of the **Oasis Infobyte Data Science Internship (OIBSIP)**.

---

## 🛠️ Tech Stack & Tools
* **Programming Language:** Python
* **Data Manipulation & Analysis:** pandas, numpy
* **Data Visualization:** matplotlib, seaborn
* **Machine Learning:** scikit-learn
* **Environment:** Jupyter Notebook

---

## 📊 Dataset Information
* **Source:** [Vehicle Dataset from CarDekho](https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho) (Kaggle)
* **Key Features:**
  * `Car_Name` / `Brand`: Brand and model of the car
  * `Year`: Year of manufacture (used to calculate `Car_Age`)
  * `Selling_Price`: Target variable (price in lakhs/thousands)
  * `Present_Price`: Original showroom price
  * `Kms_Driven`: Total distance driven
  * `Fuel_Type`: Petrol, Diesel, CNG
  * `Seller_Type`: Dealer or Individual
  * `Transmission`: Manual or Automatic

---

## ⚙️ Workflow & Feature Checklist

- [x] **Data Loading & Cleaning:**
  - Handled missing/null values and removed duplicate records.
  - Standardized inconsistent categorical text (e.g., lowercasing, stripping extra spaces).
- [x] **Feature Engineering:**
  - Extracted car brand/make from the `Car_Name` column.
  - Computed `Car_Age` ($Current\_Year - Year$) and dropped redundant raw date columns.
- [x] **Exploratory Data Analysis (EDA):**
  - Plotted distribution of selling prices.
  - Created box plots for *Price vs. Fuel Type* and *Price vs. Transmission*.
  - Visualized *Price vs. Car Age* using scatter plots.
- [x] **Data Preprocessing & Encoding:**
  - Applied One-Hot Encoding / Label Encoding on categorical variables.
  - Generated a feature correlation heatmap to analyze multicollinearity.
- [x] **Model Training & Evaluation:**
  - Split dataset into training ($80\%$) and testing ($20\%$) sets.
  - Trained multiple regression models: **Linear Regression**, **Random Forest Regressor**, and **Gradient Boosting Regressor**.
  - Evaluated performance using **Mean Absolute Error (MAE)**, **Root Mean Squared Error (RMSE)**, and **R² Score**.
- [x] **Model Insights:**
  - Visualized feature importances for the best-performing model.

---

## 📈 Model Performance & Results

| Model | MAE | RMSE | R² Score |
| :--- | :--- | :--- | :--- |
| **Linear Regression** | *[Insert MAE]* | *[Insert RMSE]* | *[Insert R²]* |
| **Random Forest Regressor** | *[Insert MAE]* | *[Insert RMSE]* | *[Insert R²]* |
| **Gradient Boosting Regressor** | *[Insert MAE]* | *[Insert RMSE]* | *[Insert R²]* |


---

