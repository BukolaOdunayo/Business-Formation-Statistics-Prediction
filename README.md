# Business-Formation-Statistics-Prediction
📌 Motivation

This project explores Business Formation Statistics (BFS) across countries to understand business activity trends and forecast future performance.
The key goal is to predict business formation in 2025Q1 using historical quarterly indicators.

We answer questions like:

1. What features are most important in predicting future business formation?

2. How accurate are machine learning models in forecasting BFS?

3. How do country effects compare with quarterly trends?

#📚 Libraries Used

Data Handling: pandas, numpy, re

Visualization: matplotlib, seaborn

#Machine Learning:

Preprocessing: StandardScaler, MinMaxScaler, OneHotEncoder, SimpleImputer, ColumnTransformer, Pipeline

Models: LinearRegression, RandomForestRegressor

Evaluation: mean_squared_error, r2_score

Environment: Jupyter Notebook

#📂 Repository Structure

BFS Data.csv → Raw dataset of Business Formation Statistics across countries.

BFS_Prediction.ipynb → Main notebook with data cleaning, EDA, feature engineering, modeling, and predictions.

README.md → Project documentation (this file)

📊 Summary of Analysis
🔹 Data Cleaning

Normalized column names, handled missing values, and converted quarter columns to numeric.

Imputed missing quarter values with column means.

Filled missing country names with the most frequent country.

🔹 Exploratory Data Analysis

Distribution plots of quarterly values.

Heatmaps showing missing values.

Correlation analysis between quarters.

🔹 Modeling

Target variable: 2025Q1

Features: Earlier quarterly indicators (2023Q2–2024Q4) + Country

Models Used:

Linear Regression

Random Forest Regressor (300 trees, random_state=42)

🔹 Results

Linear Regression: R² = 0.8475, RMSE ≈ 317,843

Random Forest: R² = 0.9761, RMSE ≈ 125,843 ✅ Best model

🔹 Feature Importance

Most predictive features: recent quarters (2024Q2–2024Q4)

Country-level features had lower influence compared to time trends.

🔹 Creative Predictive Scenario

Simulated an unseen country ("Econland") with +10% growth in 2024Q4.

Predicted 2025Q1 ≈ 21,862.

🙏 Acknowledgments

Data Source: Business Formation Statistics (BFS) dataset.

Libraries & Tools: Python scientific ecosystem (pandas, sklearn, matplotlib, etc.).

Thanks to the open-source community for building tools that make data science accessible.
