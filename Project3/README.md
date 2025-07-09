# 🛍️ Project 3: Customer Segmentation Using K-Means

## 📌 Problem Statement

Businesses need to categorize customers based on behaviors and demographics to enable better targeting, increase conversion, and improve customer satisfaction. Without segmentation, marketing efforts become generic and inefficient.

---

## 🎯 Objective

Apply **unsupervised machine learning** (K-Means) to:
- Group similar customers into meaningful clusters
- Enable data-driven personalization in marketing strategies
- Discover hidden patterns in customer behavior

---

## 📂 Dataset Overview

| Column Name        | Description                                |
|--------------------|--------------------------------------------|
| `ID`               | Unique Customer ID                         |
| `Gender`           | Male/Female                                |
| `Ever_Married`     | Marital status                             |
| `Age`              | Age of customer                            |
| `Graduated`        | Whether the customer graduated             |
| `Profession`       | Profession of the customer                 |
| `Work_Experience`  | Years of experience                        |
| `Spending_Score`   | Customer spending behavior                 |
| `Family_Size`      | Number of family members                   |
| `Var_1`            | Unknown feature (categorical)              |
| `Segmentation`     | Existing label (used only for reference)   |

---

## 🧪 Workflow

1. Merged `Train.csv` and `Test.csv` for uniform preprocessing
2. Imputed missing values using median/mode
3. Performed one-hot encoding on categorical variables
4. Scaled numerical features using `StandardScaler`
5. Used **Elbow Method** and **Silhouette Scores** to select optimal `k`
6. Applied **K-Means clustering**
7. Reduced dimensions via **PCA** for 2D and 3D plotting
8. Visualized clusters and extracted cluster-wise insights
9. Saved plots in the `plots/` directory

---

## 📈 K Selection: Silhouette Scores

| K | Silhouette Score |
|---|------------------|
| 2 | **0.2064** ✅ _(Best)_
| 3 | 0.1582           |
| 4 | 0.1392           |
| 5 | 0.1354           |
| 6 | 0.1356           |
| 7 | 0.1391           |
| 8 | 0.1319           |
| 9 | 0.1329           |

➡️ **K=2 gives the highest silhouette score**, suggesting two clearly distinguishable customer segments.

---

## 📊 Visualizations

All visuals are saved under the `plots/` folder.

- 📉 `elbow_method.png` — Elbow Curve for K selection  
- 🔷 `2d_pca_clusters.png` — 2D PCA Customer Clustering  
- 🧊 `3d_pca_clusters.html` — 3D interactive cluster visualization  

---

## 🔍 Cluster Summary (K=4 View for Reference)

| Cluster | Avg Age | Avg Work Exp | Avg Family Size | Interpretation                       |
|---------|---------|--------------|------------------|--------------------------------------|
| 0       | 51.28   | 2.17         | 3.43             | Middle-aged families, moderate work  |
| 1       | 31.70   | 2.86         | 3.01             | Young professionals, small families |
| 2       | 47.94   | 2.37         | 2.76             | Mature workers, medium households   |
| 3       | 75.46   | 1.19         | 1.98             | Seniors, low work experience         |

> ⚠️ Final clustering used **K=2**, as per silhouette results. K=4 was also analyzed for insight depth.

---

## ✅ Technologies Used

- **Python 3.10+**
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, Plotly
- **Techniques:** K-Means Clustering, PCA, Elbow Method, Silhouette Score

---
