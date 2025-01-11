# Data-Mining-Online-Retail-Customer-Segmentation

#### Online Retail Customer Segmentation Using Data Mining

#### **Overview**:
This project aims to segment customers of a UK-based online retailer using RFM metrics (Recency, Frequency, Monetary) to identify behavioral patterns and optimize targeted marketing strategies. By leveraging clustering techniques, the project provides actionable insights for improving customer engagement and maximizing revenue.

---

#### **Data Workflow**:
1. **Data Preprocessing**:
   - Handled missing `CustomerID` values.
   - Converted `InvoiceDate` to datetime format for time-based analysis.
   - Created `TotalPrice` as `Quantity × UnitPrice` for monetary value analysis.
   - Applied `StandardScaler` for data normalization.

2. **Feature Engineering**:
   - Aggregated data at the customer level using RFM metrics:
     - **Recency**: Days since the last purchase.
     - **Frequency**: Count of unique invoices.
     - **Monetary**: Total spending.

3. **Exploratory Data Analysis (EDA)**:
   - Identified seasonal trends, peak sales periods, and time-of-day activity patterns.
   - Found Q4 sales peaks and high activity on Thursday afternoons.

4. **Clustering Techniques**:
   - **K-Means Clustering**:
     - Used Elbow Method to select optimal clusters.
     - Achieved improved Silhouette Score of 0.435 after outlier removal.
   - **Hierarchical Clustering**:
     - Validated results with Ward Linkage dendrogram, achieving Silhouette Score of 0.588.

---

#### **Technologies and Tools**:
- **Programming**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Algorithms**: K-Means, Agglomerative Clustering
- **Evaluation Metrics**: Silhouette Score, Cohesion-Separation Ratio

---

#### **Results and Insights**:
- Segmented customers into three groups:
  - **High-Value, Loyal Customers**: Frequent buyers with significant spending.
  - **Moderate Buyers**: Regular customers with consistent but average spending.
  - **Inactive Buyers**: Infrequent purchasers with minimal engagement.
- Delivered strategies for tailored marketing:
  - Loyalty programs for high-value customers.
  - Personalized offers for moderate buyers.
  - Re-engagement campaigns for inactive customers.

---

#### **How to Run**:
1. Clone the repository:
   ```bash
   git clone <repository-link>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook:
   ```bash
   jupyter notebook Online_Retail_Segmentation.ipynb
   ```

---
