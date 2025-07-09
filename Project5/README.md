# 🧮 E-Commerce Purchase Prediction using Gradient Descent

## 📌 Problem Statement

E-commerce platforms need to estimate how much users are likely to spend based on product categories, demographics, and payment behavior. Accurate predictions enable better inventory management, targeted promotions, and customer segmentation.

---

## 🎯 Objective

Build a **Linear Regression model from scratch** using **Gradient Descent** to predict the `Purchase_Amount` per transaction, and extract key revenue-driving insights such as:

- High-value product categories
- Country-wise purchasing patterns

---

## 📂 Dataset Overview

| Column Name        | Description                                      |
|--------------------|--------------------------------------------------|
| `Transaction_ID`   | Unique transaction identifier                    |
| `User_Name`        | Name of the customer                             |
| `Age`              | Age of the customer                              |
| `Country`          | Country where the purchase was made              |
| `Product_Category` | Category of the purchased product                |
| `Purchase_Amount`  | Total amount spent (target variable)             |
| `Payment_Method`   | Method used for payment (Card, Wallet, etc.)     |
| `Transaction_Date` | Date and time of the transaction                 |

---

## 🧪 Workflow

1. Loaded and encoded the dataset
2. Applied one-hot encoding on categorical features
3. Scaled the data using `StandardScaler`
4. Implemented custom gradient descent algorithm
5. Predicted `Purchase_Amount` and evaluated training loss
6. Extracted **top-grossing product categories per country**

---

## 📉 Gradient Descent Training Summary

| Epoch | Loss      | Bias (b) |
|-------|-----------|----------|
| 1     | 335,286.81 | 10.0632  |
| 2     | 325,204.50 | 19.9251  |
| 3     | 315,521.51 | 29.5898  |
| 4     | 306,222.01 | 39.0612  |
| 5     | 297,290.81 | 48.3432  |
| 6     | 288,713.32 | 57.4395  |
| 7     | 280,475.55 | 66.3539  |
| 8     | 272,564.03 | 75.0900  |
| 9     | 264,965.84 | 83.6514  |
| 10    | 257,668.57 | 92.0416  |

➡️ Training loss decreased consistently, indicating convergence.

---

## 🌍 Top Revenue-Generating Product Category per Country

| Country   | Top Product Category | Total Purchase Amount |
|-----------|----------------------|------------------------|
| Australia | Grocery              | 335,303.16             |
| Brazil    | Clothing             | 333,614.47             |
| Canada    | Books                | 340,734.15             |
| France    | Clothing             | 331,622.23             |
| Germany   | Sports               | 326,127.36             |
| India     | Electronics          | 329,364.17             |
| Japan     | Beauty               | 323,443.64             |
| Mexico    | Toys                 | 339,836.63             |
| UK        | Sports               | 334,038.64             |
| USA       | Home & Kitchen       | 328,129.75             |

These insights help prioritize stock and tailor promotions by region.

---

## ✅ Technologies Used

- Python
- Pandas, NumPy
- scikit-learn (for scaling)
- Manual NumPy-based Gradient Descent

---


