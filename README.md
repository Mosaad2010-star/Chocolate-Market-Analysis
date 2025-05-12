# 🍫 Chocolate Sales Analysis & Forecasting

This project provides a comprehensive data analysis and forecasting workflow on chocolate sales data. The goal was to uncover actionable insights, build predictive models, and offer strategic business recommendations.

## 📌 Project Objectives

- Understand and clean raw sales data
- Perform exploratory data analysis (EDA)
- Predict future sales using machine learning
- Forecast long-term trends using time series models
- Provide business recommendations based on findings

---

## 🔍 1. Data Understanding & Cleaning

- **Loaded Dataset:** `Chocolate Sales.csv` with key columns: `Sales Person`, `Country`, `Product`, `Date`, `Amount`, and `Boxes Shipped`.
- **Cleaning Steps:**
  - Removed `$` and commas from `Amount`, converted to numeric.
  - Converted `Date` to datetime format.
  - Ensured `Boxes Shipped` is numeric and handled missing values.
  - Applied z-score for outlier removal.
  - Extracted `year`, `month`, `day`, `weekday` for time-based features.
  - Encoded categorical features for modeling.

---

## 📊 2. Exploratory Data Analysis (EDA)

- **Sales Over Time:** Visualized total sales trends and seasonality.
- **By Country:** Aggregated and compared sales volume.
- **By Product:** Identified best-selling and highest-value products.
- **Shipping Insights:** Analyzed logistics efficiency by correlating boxes shipped vs. revenue.
- **Sales Person Performance:** Compared total sales and shipping performance per representative.
- **Seasonality:** Monthly trends plotted with seasonal decomposition.

---

## 🤖 3. Predictive Modeling

### Regression
- **Goal:** Predict `Amount` using:
  - Linear Regression
  - Random Forest Regressor
  - XGBoost Regressor
- **Evaluation:** R² score

### Classification
- **Goal:** Classify each sale as `High` or `Low` (based on median value)
  - Logistic Regression
  - Random Forest Classifier
- **Metrics:** Accuracy and classification report

---

## ⏳ 4. Time Series Forecasting

- **Tool:** [Facebook Prophet](https://facebook.github.io/prophet/)
- **Goal:** Forecast daily sales for upcoming 3 months
- **Result:** Forecast plot + decomposition (trend, seasonality)

---

## 💡 5. Key Insights & Recommendations

### 📈 Insights
- **Top Countries** by total revenue
- **Top Salespersons** based on performance
- **Popular Products** and best-selling combinations
- **Clear Seasonality** trends in monthly sales

### 🧭 Recommendations
- Focus investment in high-performing markets
- Launch promotional bundles using best-seller combinations
- Plan logistics around seasonal demand peaks
- Improve operations in underperforming regions

---

## 📂 Project Structure

