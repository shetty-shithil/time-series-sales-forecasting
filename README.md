# 📊 Store Sales Forecasting & Business Performance Analysis

## 📌 Project Overview

This project analyzes historical retail sales and profitability data to uncover trends, regional disparities, and product-level performance drivers. Using **interactive Tableau dashboards** and an **XGBoost-based forecasting model**, the analysis enables stakeholders to assess past performance, diagnose profitability risks, and anticipate future demand.

Three integrated dashboards were developed:

1. **Business Performance Overview**
2. **Product & Profitability Analysis**
3. **Sales Forecasting & Future Demand Outlook**

Together, these dashboards form a cohesive **decision-support system** that transforms transactional data into actionable business insights.

---

## 🎯 Problem Statement

Organizations often track sales performance without fully understanding the interaction between profitability, growth trends, and regional or product-level variations. High revenue does not necessarily imply high profit, and underperforming regions or product categories may remain unnoticed until their financial impact becomes significant.

This project addresses the challenge of **analyzing sales, profit, and growth simultaneously** to identify strengths, risks, and opportunities across time, geography, and product categories.

---

## 🎯 Project Objectives

- Analyze historical sales and profit trends  
- Compare revenue growth with profitability behavior  
- Identify high- and low-performing regions and product sub-categories  
- Deliver insights through intuitive, interactive Tableau dashboards  
- Extend descriptive insights into the future using machine learning–based forecasting  

---

## 📎 Data Source

**Kaggle – Store Sales Forecasting Dataset**  
https://www.kaggle.com/datasets/tanayatipre/store-sales-forecasting-dataset/data

**Key Fields:**
- Order date  
- Sales revenue  
- Profit  
- Product sub-category  
- Region and state  

---

## 🧹 Data Preparation & Feature Engineering

The dataset was prepared to ensure analytical accuracy and suitability for both descriptive and predictive modeling:

- Standardized date fields for weekly, monthly, and yearly analysis  
- Validated sales and profit records and handled missing values  
- Aggregated data across region, product, and time dimensions  

**Derived Metrics:**
- Profit margin (Profit / Sales)  
- Year-over-Year (YoY) sales growth  
- Sales and profit moving averages  

**Forecasting Preparation:**
- Weekly aggregation of historical sales  
- Time-based feature engineering to capture trend and seasonality  
- Temporal train–validation split to prevent data leakage  

An **XGBoost regression model** was used to forecast weekly sales for the next ten weeks, leveraging its ability to model non-linear patterns and complex interactions.

---

## 📊 Dashboard 1: Business Performance Overview

### Objective
Provide a high-level view of business performance by combining **sales growth, profitability trends, and regional analysis**.

### Key Insights
- Sales exhibit strong seasonality, while profit remains volatile  
- Revenue growth moderated after an initial peak  
- Performance varies significantly by region  
- Certain regions generate revenue at the expense of profitability  

This dashboard supports executive-level assessment of growth sustainability and regional risk.

---

## 📦 Dashboard 2: Product & Profitability Analysis

### Objective
Explain **what drives profitability and loss at the product sub-category level**.

### Key Insights
- Sales are concentrated within a small set of sub-categories  
- High sales do not always correspond to high profit  
- Some sub-categories are structurally margin-negative  
- Profit stability varies widely across products  

This dashboard informs pricing strategy, promotion decisions, and product portfolio optimization.

---

## 🔮 Dashboard 3: Sales Forecasting & Future Demand Outlook (XGBoost)

### Objective
Provide a forward-looking view of demand by forecasting **weekly sales for the next ten weeks**.

### Methodology
- Trained an XGBoost model on historical weekly sales  
- Captured seasonality and short-term demand patterns  
- Validated forecasts against historical data  

### Key Insights
- XGBoost effectively models short-term sales trends  
- Future demand remains concentrated in key sub-categories  
- Regional demand projections enable proactive planning  
- Forecast uncertainty varies across product categories  

This dashboard enables **data-driven demand planning and risk-aware decision-making**.

---

## 🧠 End-to-End Analytical Storyline

- **Descriptive:** How has the business performed historically?  
- **Diagnostic:** Where are profits created or lost today?  
- **Predictive:** What is likely to happen next, and how should the business prepare?  

This progression aligns with modern **business intelligence and analytics best practices**.

---

## 🛠 Tools & Technologies

- **Tableau:** Interactive dashboards and visual analytics  
- **XGBoost:** Machine learning–based sales forecasting  
- **Python:** Data preparation and feature engineering  

---

## ✅ Key Takeaways

- Revenue growth must be evaluated alongside profitability  
- Regional and product-level heterogeneity strongly impact performance  
- Machine learning enhances short-term demand forecasting  
- Tableau dashboards translate analytics into actionable insights  
