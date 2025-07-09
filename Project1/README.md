# 🛍️ Sales Forecasting with Linear Regression

This project analyzes sales data and builds a linear regression model to forecast sales. It includes data preprocessing, exploratory data analysis (EDA), and model building using scikit-learn pipelines.

## 📁 Dataset

The dataset used for this project contains historical sales records, including customer details, product categories, and order/ship dates.

- 📅 **Order Date**
- 🚚 **Ship Date**
- 📦 **Sales**
- 🌍 **Region**, **City**, **Postal Code**
- 👤 **Customer Name**, **Segment**
- 📦 **Category**, **Sub-Category**, **Product ID**

---

## 📊 Exploratory Data Analysis (EDA)

1. **Customer Segment Distribution**  
   Pie chart showing the distribution of customers among different business segments.

2. **Monthly Sales Trend**  
   Line plot showing how sales evolve month-over-month.

3. **Total Sales by Region**  
   Horizontal bar plot ranking regions by total sales.

4. **Time Taken by Different Ship Modes**  
   Scatter plot of average processing times per ship mode.

5. **Most Valuable Customers**  
   Bar chart displaying the top 20 revenue-generating customers.

6. **Sub-Category Distribution per Category**  
   Count plot visualizing sub-categories across each product category.

7. **Top 10 Cities by Sales**  
   Bar plot of cities that contribute the most to sales.

8. **Correlation Matrix**  
   Heatmap showing correlations among numeric features.

---

## 🧼 Data Preprocessing

- Converted `Order Date` and `Ship Date` to datetime objects.
- Calculated `Processing Time` as difference in days between ship and order dates.
- Handled missing values in `Postal Code`.
- Removed outliers from the `Sales` column using the 1st and 99th percentiles.
- Added `Order_Year` and `Order_Month` features.
- Used one-hot encoding for categorical columns.
- Applied `StandardScaler` and `SimpleImputer` in a pipeline.

---

## 🔮 Model: Linear Regression

A `Pipeline` was built using:

- **Preprocessing:**
  - `SimpleImputer` for missing values.
  - `StandardScaler` for numeric columns.
  - `OneHotEncoder` for categorical columns.
- **Model:** `LinearRegression`

### 🔧 Train-Test Split

- 80% training, 20% testing
- `Log1p` transformation on `Sales` for improved linearity

---

## 📈 Evaluation Metrics

| Metric | Value |
|--------|-------|
| R² Score | **0.3164** |
| MAE      | **110.07** |
| MSE      | **67796.89** |

### 📉 Actual vs Predicted Plot

A line plot comparing actual and predicted values for the first 100 rows was saved to:

