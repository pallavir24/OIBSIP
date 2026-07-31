# Task 5: Sales Prediction Using Python

## 📌 Project Overview
This project builds a regression model to predict product sales based on advertising expenditures across different media channels (**TV**, **Radio**, and **Newspaper**). By analyzing historical advertising data, we identify which marketing channels drive the highest return on investment and optimize future ad budget allocations.

---

## 🛠️ Tech Stack & Tools
* **Language:** Python
* **Data Manipulation:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`
* **Machine Learning:** `scikit-learn`
* **Environment:** Google Colab

---

## 🚀 Workflow & Features

1. **Exploratory Data Analysis (EDA):**
   * Handled missing values and verified data integrity.
   * Generated descriptive statistics for feature distributions.
   * Plotted `pairplot` and individual scatter plots (`Sales` vs. `TV`, `Radio`, `Newspaper`).
   * Evaluated feature correlations using a heatmap.

2. **Model Training & Evaluation:**
   * Split data into **80% Training** and **20% Testing** sets.
   * Trained a baseline **Linear Regression** model.
   * Trained an advanced **Random Forest Regressor** to evaluate non-linear patterns.
   * Evaluated performance using:
     * Mean Absolute Error (**MAE**)
     * Root Mean Squared Error (**RMSE**)
     * Coefficient of Determination (**$R^2$ Score**)

3. **Model Diagnostics & Feature Importance:**
   * Analyzed residual plots to ensure errors are randomly distributed without systematic bias.
   * Evaluated feature coefficients and feature importance to pinpoint high-impact channels.

---

## 📊 Model Performance

| Model | MAE | RMSE | $R^2$ Score |
| :--- | :--- | :--- | :--- |
| **Linear Regression (Baseline)** | *[Insert MAE]* | *[Insert RMSE]* | *[Insert R²]* |
| **Random Forest Regressor** | *[Insert MAE]* | *[Insert RMSE]* | *[Insert R²]* |

*(Note: Replace bracketed values above with your actual model results.)*

---

## 💡 Key Insights & Business Takeaways
* **Primary Driver:** **TV advertising** shows the strongest positive correlation with sales, making it the most impactful media channel for boosting revenue.
* **Secondary Channel:** **Radio advertising** exhibits a moderate positive effect on sales and works best when paired with TV campaigns.
* **Low-Impact Channel:** **Newspaper advertising** has minimal impact on overall sales performance, suggesting that budget from newspaper ads can be reallocated to TV/Radio for better ROI.

---

## 📂 Repository Structure
```text
.
├── Advertising.csv                           # Dataset
├── Sales_Prediction_Using_Python.ipynb        # Main Jupyter Notebook
└── README.md                                 # Project documentation
