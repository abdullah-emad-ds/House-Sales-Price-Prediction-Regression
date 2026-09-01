# 🏡 King County House Sales Price Prediction & Regression Modeling

## 📌 Project Overview
A machine learning project focused on predictive modeling and price valuation for residential properties sold in King County, Washington (including Seattle). The project applies Exploratory Data Analysis (EDA), feature engineering, missing data imputation, and multiple regression algorithms to maximize price estimation accuracy ($R^2$).

## 🛠️ Tech Stack & Methods
* **Programming & Libraries:** Python, Pandas, NumPy, Matplotlib, Seaborn
* **Machine Learning (Scikit-Learn):** Linear Regression, Ridge Regression ($\text{L2}$ Regularization), Polynomial Features, `StandardScaler`, `Pipeline`, `train_test_split`, `cross_val_score`
* **Evaluation Metrics:** Coefficient of Determination ($R^2$ Score)

---

## 🔬 Workflow & Modeling Pipeline
1. **Data Wrangling & Cleaning:** Handled missing values via mean imputation across bedroom and bathroom attributes; dropped redundant identifier columns.
2. **Exploratory Data Analysis (EDA):** Evaluated feature correlations with property prices, generating regression plots (`regplot`) and box plots for waterfront view, living area (`sqft_living`), and construction grade.
3. **Model Development & Benchmarks:**
   * **Simple Linear Regression:** Baseline evaluation on single geographic/structural attributes.
   * **Multi-variable Linear Regression:** Features including `grade`, `bathrooms`, `sqft_above`, `lat`, and `view` ($R^2 \approx 0.658$).
   * **Scikit-Learn Pipeline with Polynomial Features (Degree 2) + Scaling:** Boosted model performance to $R^2 \approx 0.751$.
   * **Ridge Regularization ($\alpha = 0.1$):** Controlled overfitting on high-dimensional polynomial features ($R^2 \approx 0.700$ on held-out test data).

---

## 🚀 How to Run Locally
1. Clone the repository:
   ```bash
   git clone [https://github.com/abdullah-emad-ds/House-Sales-Price-Prediction-Regression.git](https://github.com/abdullah-emad-ds/House-Sales-Price-Prediction-Regression.git)
