# 📈 Sales Forecasting Using XGBoost

## 📌 Project Overview

This project focuses on forecasting retail store sales using historical transaction data and machine learning techniques. Leveraging **XGBoost**, a powerful gradient boosting algorithm, the goal is to accurately predict future sales by capturing seasonal trends, temporal dependencies, and store-level patterns.

In addition to predictive modeling, **interactive Tableau dashboards** were built to visualize sales trends, forecast results, and store-level performance, enabling stakeholders to explore insights intuitively and support data-driven planning.

---

## 🧠 Methodology

### 1️⃣ Data Preparation & Exploratory Data Analysis (EDA)

- Parsed and validated date fields  
- Checked for missing values, outliers, and inconsistencies  
- Analyzed:
  - Sales trends over time  
  - Store-level sales distributions  
  - Seasonality and demand fluctuations  
- Visualized daily, weekly, and monthly sales patterns  

---

### 2️⃣ Feature Engineering

- Extracted time-based features:
  - Year, month, week, day of week  
  - Is_weekend / is_holiday indicators (if applicable)  
- Created lag features:
  - Previous day, week, and rolling-window sales  
- Generated rolling statistics:
  - Moving averages  
  - Rolling standard deviation  
- Encoded categorical variables (e.g., store ID)  

---

### 3️⃣ Modeling & Forecasting

- Implemented **XGBoost Regressor** for sales prediction  
- Used time-aware train–test splits to prevent data leakage  
- Tuned hyperparameters:
  - Learning rate  
  - Max depth  
  - Number of estimators  
- Generated short-term sales forecasts at the store level  

---

### 4️⃣ Model Evaluation

- Evaluated model performance using:
  - RMSE (Root Mean Squared Error)  
  - MAE (Mean Absolute Error)  
- Compared actual vs predicted sales  
- Analyzed residual patterns across time and stores  

---

### 5️⃣ Visualization & Interpretation

- Time series plots of actual vs predicted sales  
- XGBoost feature importance analysis  
- Error trends and forecast stability assessment  
- Focused on interpretability and business relevance  

---

## 📊 Tableau Dashboards

Developed **interactive Tableau dashboards** to complement the forecasting model and communicate insights effectively:

- 📈 **Sales Trends Dashboard**  
  Visualizes historical sales patterns, seasonality, and growth trends across stores and time.

- 🔮 **Forecast vs Actual Dashboard**  
  Compares predicted sales against actual values, highlighting forecast accuracy and deviations.

- 🏬 **Store Performance Dashboard**  
  Enables store-level analysis with filters for date ranges and sales metrics to identify high- and low-performing locations.

These dashboards allow non-technical stakeholders to explore forecasts, monitor performance, and support planning decisions.

---

## 🔍 Key Insights

- XGBoost successfully captured **seasonal patterns and short-term sales dependencies**  
- Lag and rolling-window features were among the strongest predictors  
- Store-level sales behavior varied significantly, reinforcing the need for granular forecasting  
- Tableau dashboards enhanced interpretability and accessibility of model outputs  

---

## 📎 Dataset Source

**Kaggle – Store Sales Forecasting Dataset**  
https://www.kaggle.com/datasets/tanayatipre/store-sales-forecasting-dataset/data
