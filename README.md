# Online Retail Data Clustering

This project performs customer segmentation using clustering techniques on an online retail dataset. The primary objective is to identify different customer groups based on purchasing behavior to improve marketing strategies and decision-making.

## Project Structure

- `Online Retail Data Clustering.ipynb`: Jupyter notebook containing the entire workflow — from data preprocessing to model building and visualization.
- The dataset typically includes customer transactions for a UK-based online retailer.

## Key Steps

### 1. **Data Preprocessing**
- Loaded the online retail data.
- Removed missing and invalid entries.
- Filtered out canceled transactions.
- Removed negative or zero quantities and prices.

### 2. **Feature Engineering**
- Grouped data by `CustomerID`.
- Calculated:
  - **Recency**: Days since last purchase.
  - **Frequency**: Total number of purchases.
  - **Monetary**: Total amount spent.

### 3. **EDA (Exploratory Data Analysis)**
- Histograms and boxplots for RFM features.

### 4. ** Feature Scaling
- StandardScaler used for feature scaling.

### 5. **Clustering**
- Applied **KMeans Clustering** on scaled RFM data.
- Used **Elbow Method** and **Silhouette Score** to find optimal clusters.
- Chose the best `k` value for customer segmentation.
- Visualized clusters using voilinplots and 3D scatter plots.

### 6. **Insights**
- Cluster profiles revealed different customer types:
  - High spenders with frequent purchases.
  - Infrequent but high-value buyers.
  - Low-value or inactive customers.

##  Results

- Optimal number of clusters: **4** (based on Elbow method).
- Clear segmentation achieved.
- Cluster-wise characteristics are interpretable and usable for business decisions.
