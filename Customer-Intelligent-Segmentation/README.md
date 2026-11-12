# 🛍️ Intelligent Customer Segmentation for Marketing

## 📌 Project Overview

This project focuses on developing an intelligent customer segmentation system using Unsupervised Machine Learning.
It applies the K-Means Clustering algorithm to group retail customers based on their Annual Income and Spending Score.
The system identifies different customer segments and provides targeted marketing recommendations to help businesses understand customer behaviour, improve marketing strategies, and allocate promotional resources effectively.

## 🎯 Objectives

- Analyse customer purchasing behaviour and income patterns.
- Perform data preprocessing and exploratory data analysis.
- Apply K-Means clustering to identify customer segments.
- Determine the optimal number of clusters using the Elbow Method and Silhouette Score.
- Develop targeted marketing strategies for each customer segment.

## 📊 Dataset Description

**Dataset:** Mall Customer Segmentation Dataset

- Total Records: 200 customers
- Total Attributes: 5

| Feature | Description |
|---|---|
| CustomerID | Unique customer identifier |
| Gender | Male / Female |
| Age | Customer age |
| Annual Income (k$) | Annual income in thousands |
| Spending Score (1–100) | Customer spending behaviour |

For clustering, the following two features were selected:
- Annual Income (k$)
- Spending Score (1–100)

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Platform:** Google Colab
- **Libraries:**
  - Pandas
  - NumPy
  - Matplotlib
  - Seaborn
  - Scikit-learn

## ⚙️ Methodology

1. **Data Collection:** Load the Mall Customer Segmentation dataset.
2. **Data Preprocessing:** Check missing values and remove the CustomerID column.
3. **Feature Selection:** Select Annual Income and Spending Score.
4. **Feature Scaling:** Apply StandardScaler to normalize numerical features.
5. **Model Building:** Implement the K-Means clustering algorithm.
6. **Optimal Cluster Selection:** Use the Elbow Method and Silhouette Score.
7. **Model Validation:** Evaluate the clustering performance.
8. **Customer Profiling:** Identify customer groups and recommend marketing strategies.

## 🤖 Algorithm Used

**K-Means Clustering**

K-Means is an unsupervised machine learning algorithm that groups similar data points into clusters based on their distance from cluster centres.

The optimal number of clusters identified for this project is **K = 5**.

## 📈 Results

The model successfully identified five distinct customer segments.

| Cluster | Customer Segment |
|---|---|
| 0 | Mid-Range Mixed Spenders |
| 1 | Premium Champions |
| 2 | Low-Income High Spenders |
| 3 | Cautious Affluents |
| 4 | Budget Shoppers |

### Model Performance

- Optimal Clusters: 5
- Silhouette Score: 0.5547
- Inertia (WCSS): 65.57
- Algorithm: K-Means Clustering

### Marketing Insights

- **Premium Champions:** VIP rewards, early product access, and exclusive promotions.
- **Cautious Affluents:** Trust-building campaigns and quality assurance.
- **Low-Income High Spenders:** Loyalty schemes and budget-friendly premium bundles.
- **Budget Shoppers:** Discount coupons, value deals, and price alerts.
- **Mid-Range Mixed Spenders:** Personalized offers, cross-selling, and membership rewards.

## 🔍 Key Findings

- Annual Income and Spending Score are important features for customer segmentation.
- Five meaningful customer groups were identified.
- High-income customers do not necessarily have high spending scores.
- K-Means clustering helps businesses understand different customer behaviours.
- Segment-based marketing strategies can improve promotional effectiveness.

## 🚀 Future Scope

- Incorporate additional features such as Age and Gender.
- Explore advanced clustering algorithms such as DBSCAN, GMM, and Hierarchical Clustering.
- Develop a web application using Streamlit or Flask.
- Integrate A/B testing to evaluate the impact of targeted marketing campaigns.

---

⭐ *This project demonstrates the application of unsupervised machine learning in customer behaviour analysis and data-driven marketing decision-making.*
