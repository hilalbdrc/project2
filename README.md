# Customer Segmentation with K-Means Clustering

This project focuses on analyzing customer behavior and grouping customers into distinct segments using machine learning. By leveraging **RFM (Recency, Frequency, Monetary)** metrics and **K-Means Clustering**, the project aims to provide actionable insights for data-driven marketing strategies.

## 📌 Project Overview
The analysis is performed on a retail dataset to understand customer purchasing patterns. The workflow includes comprehensive data cleaning, feature engineering, and the application of unsupervised learning algorithms to identify high-value customers and those at risk of churn.

## 🚀 Key Features & Methodology
- **Exploratory Data Analysis (EDA):** Detailed profiling of the dataset, handling missing values, and identifying statistical anomalies.
- **Data Preprocessing:** - Filtering canceled transactions and outliers.
  - Advanced feature engineering (Total Price calculation, Date-time formatting).
  - Outlier handling using the Interquartile Range (IQR) method.
- **RFM Analysis:** Transformation of raw transactional data into Recency, Frequency, and Monetary scores.
- **Machine Learning (Clustering):**
  - Data normalization using `StandardScaler`.
  - Determining the optimal number of clusters using the **Elbow Method**.
  - Customer segmentation with **K-Means**.
- **Visualizations:** Interactive and static plots including Elbow curves, 3D cluster visualizations, and segment distributions.
### 1. Dimensionality Reduction (PCA)
- Applied **Principal Component Analysis (PCA)** to simplify complex customer features while retaining maximum variance.
- Visualized high-dimensional data in 2D/3D to confirm the natural separation of customer clusters.
### 2. Behavioral Segmentation (K-Means)
Identified **4 distinct customer segments** using RFM metrics:
- **VIP Customers (Cluster 3):** High-value, high-frequency "Champions."
- **Loyal Customers (Cluster 1):** Consistent shoppers with steady engagement.
- **Potential Loyalists (Cluster 2):** Recent customers with growing transaction volume.
- **At Risk / Lost (Cluster 4):** Customers showing signs of churn.
### 3. Cohort Analysis
- Performed **Time-based Cohort Analysis** to track customer retention over months.
- Analyzed how different "join dates" impact long-term purchasing behavior.
### 4. CLTV Prediction (BG/NBD & Gamma-Gamma)
- **BG/NBD Model:** Used to predict the expected number of transactions from each customer in the next 3-6 months.
- **Gamma-Gamma Submodel:** Used to estimate the average transaction value.
- Combined these to calculate the **Customer Lifetime Value**, ranking customers by their future profit potential.
### 5. New Customer Prediction Pipeline
- Built a functional prediction script that takes **Recency, Frequency, and Monetary** inputs for a new customer and automatically assigns them to one of the 4 pre-defined segments.

## 🛠️ Tech Stack
- **Language:** Python 3.14.0
- **Libraries:**
  - `pandas` & `numpy`: Data manipulation
  - `matplotlib` & `seaborn`: Data visualization
  - `scikit-learn`: Machine learning and preprocessing
  - `squarify`: Treemap visualizations for segments

## 📈 Results & Business Insights
The model segments customers into 4 primary groups based on their behavioral patterns:
- **VIP Customers:** Top-tier spenders with high engagement.
- **Loyal Customers:** Reliable shoppers with consistent purchase history.
- **Potential Loyalists:** New or moderate shoppers with high potential for growth.
- **At Risk/Lost:** Customers showing signs of churn who need re-engagement.
- **Efficiency:** PCA reduced feature noise, leading to more stable clusters.
- **Retention:** Cohort heatmaps identified critical months where customer drop-off is highest.
- **Revenue:** CLTV scores allow for "Value-Based Marketing," prioritizing high-potential customers for premium campaigns.


## 📬 Contact
**Hilal Biderci** *Industrial Engineer & Machine Learning Researcher* [LinkedIn Profile](https://www.linkedin.com/in/drhilalbiderci/) | [GitHub](https://github.com/drhilalbiderci)