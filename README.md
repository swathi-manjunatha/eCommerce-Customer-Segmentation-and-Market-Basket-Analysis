# 🛒 Customer Segmentation & Market Basket Analysis

## 📌 Project Overview
This project explores customer behavior and product affinity using transactional data from a UK-based online retailer. Through data preprocessing, segmentation, and association rule mining, the goal is to extract actionable insights to improve customer targeting and cross-selling strategies.

---

## 📊 Dataset
- **Source**: UK-based online retail dataset (public domain)
- **Records**: 500,000+ transactions
- **Customers**: ~35,000 unique
- **Time Period**: December 2010 – December 2011
- **Features**: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country

---

## 🧪 Techniques Used

### 🔹 Customer Segmentation
- **RFM Analysis**: Segmented customers based on Recency, Frequency, and Monetary value.
- **Clustering**: Applied **K-Means** and **Hierarchical Clustering** (validated with Elbow Method & Silhouette Score) to identify distinct customer groups.

### 🔹 Market Basket Analysis
- Transformed transactional data into a **basket format**.
- Used the **Apriori algorithm** to mine frequent itemsets and generate association rules.
- Extracted rules with **lift > 2.5** to uncover high-lift product pairings for cross-selling.

---

## 📈 Key Insights
- Top 20% of customers contributed to ~65% of revenue.
- Identified 5 high-value customer clusters for targeted marketing.
- Discovered 50+ strong product associations, revealing bundles that could increase average order value by ~15%.
- Insights help simulate loyalty programs, promotional strategies, and product placement decisions.

---

## 🧰 Tech Stack
- **Python**: `pandas`, `numpy`, `seaborn`, `matplotlib`
- **Machine Learning**: `scikit-learn` (clustering), `mlxtend` (Apriori)
- **Visualization**: Seaborn, Matplotlib
- **Jupyter Notebook**

---

## 🚀 How to Run the Project

1. Clone this repository:
```bash
git clone https://github.com/your-username/customer-segmentation.git
cd customer-segmentation
