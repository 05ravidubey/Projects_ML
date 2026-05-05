Customer Segmentation using K-Means Clustering

Overview
This project applies **K-Means Clustering** to segment customers based on their purchasing behavior. The goal is to identify distinct customer groups using **Annual Income** and **Spending Score**, enabling targeted marketing and business strategies.
Problem Statement
Businesses often struggle to understand customer behavior. This project answers:

* Who are the most valuable customers?
* Which customers should be targeted?
* How can marketing strategies be optimized?

Dataset

Name:Mall_Customers Dataset
  
  Features:

  * CustomerID
  * Gender
  * Age
  * Annual Income (k$)
  * Spending Score (1–100)

 Project Pipeline

1. Data Loading

* Loaded dataset using Pandas

2. Data Cleaning

* Removed `CustomerID` (non-informative)
* Checked for missing values

3. Feature Engineering

Encoded Gender:

  * Male → 1
  * Female → 0

4. Feature Scaling

* Applied **StandardScaler**
* Important for distance-based algorithms like K-Means

5. Optimal Cluster Selection

Elbow Method

Silhouette Score

6. Model Training

* Applied K-Means with:

  ```python
  n_clusters = 5
  ```

7. Visualization

* Scatter plot: Income vs Spending Score
* Cluster coloring
* Centroid visualization

8. Cluster Analysis

* Used:

  python
  df.groupby("Cluster").mean()
  
* Interpreted customer profiles
Results

Customer Segments Identified

| Cluster   | Description                                         |
| --------- | ----------------------------------------------------|
| Cluster 0 | Average customers (medium income & spending)        |
| Cluster 1 | High income, high spending (**Premium customers**)  |
| Cluster 2 | Low income, high spending (Impulsive buyers)        |
| Cluster 3 | High income, low spending (**Target segment**)      |
| Cluster 4 | Low income, low spending (Low-value customers)      |

 Key Insights

* High income ≠ high spending
* **Cluster 3** is the most important segment for growth
* **Cluster 1** contributes maximum revenue
* Gender does not significantly influence clustering

Conclusion

K-Means clustering successfully identified meaningful customer segments, enabling data-driven business decisions and targeted marketing strategies.
