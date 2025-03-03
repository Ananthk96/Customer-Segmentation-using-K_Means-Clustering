
# Customer Segmentation Using K-Means Clustering

## Project Overview

This project focuses on **customer segmentation** using **K-Means clustering** to analyze and categorize customers based on their purchasing behavior. The goal is to identify distinct customer groups and develop targeted business strategies to enhance customer engagement, retention, and revenue growth.

---

## Key Steps Performed

### 1. **Data Import and Cleaning**
   - Imported the dataset and performed data cleaning.
   - Corrected data types and removed canceled transactions and null customer IDs.

### 2. **Revenue Calculation**
   - Created a new `Revenue` column by multiplying `Price` and `Quantity`.

### 3. **Customer-Level Metrics**
   - Aggregated customer-level metrics including:
     - **Monetary Value**: Total revenue per customer.
     - **Frequency**: Number of unique invoices per customer.
     - **Recency**: Most recent purchase date per customer.

### 4. **Outlier Detection and Treatment**
   - Identified and separated outliers in `Monetary Value` and `Frequency`.
   - Used the **Interquartile Range (IQR)** method to detect and handle outliers.

### 5. **Data Scaling**
   - Scaled the data using `StandardScaler` to normalize the features for clustering.

### 6. **K-Means Clustering**
   - Applied the **Elbow Method** to determine the optimal number of clusters.
   - Used **Silhouette Score** to validate the clustering quality.
   - Visualized clusters in a **3D scatter plot**.

### 7. **Cluster Analysis and Business Strategies**
   - Identified four main customer clusters:
     - **Cluster 0 (ADDRESS)**: High-value, inactive customers.
     - **Cluster 1 (ENGAGE)**: Low-value, recent customers.
     - **Cluster 2 (NURTURE)**: Low-value, infrequent but recent customers.
     - **Cluster 3 (PRIORITY)**: High-value, frequent, and recent customers.
   - Developed tailored business strategies for each cluster to maximize customer value and engagement.

### 8. **Outlier Cluster Strategies**
   - Addressed outliers with specific strategies:
     - **Cluster -1 (PAMPER)**: High spenders with infrequent purchases.
     - **Cluster -2 (UPSELL)**: Frequent buyers with low spending.
     - **Cluster -3 (BURGUNDY)**: Top-tier customers with high spending and frequency.
       
![image](https://github.com/user-attachments/assets/e6886083-6a48-4f59-845d-50c452537d48)

---

## Tools and Technologies

- **Python**: Data manipulation and analysis.
- **Pandas**: Data cleaning and aggregation.
- **Scikit-learn**: K-Means clustering and data scaling.
- **Matplotlib/Seaborn**: Data visualization.
- **Google Colab**: Notebook environment for development.

---

## Possible Business Impact

- **Enhanced Customer Retention**: Targeted strategies for each cluster to improve customer loyalty.
- **Increased Revenue**: Upselling and cross-selling opportunities identified through segmentation.
- **Data-Driven Decision Making**: Insights derived from customer behavior to inform marketing and sales strategies.

---

## Future Work

- Explore advanced clustering techniques like DBSCAN or hierarchical clustering.

---

