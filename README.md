# Customer Segmentation and Outlier Handling in Retail Data

## Overview

This project performs customer segmentation on retail transaction data using clustering techniques, with a focus on handling outliers and improving the quality of the analysis. The dataset used contains information about customer purchases, including quantities, prices, and other transactional details.

### Project Overview

The goal of this project is to:

- Clean and preprocess the data by handling missing values, duplicate records, and outliers.
- Perform an exploratory data analysis (EDA) to summarize key statistics, revenue distribution, and customer behavior.
- Apply clustering techniques (KMeans and Hierarchical Clustering) to segment customers based on their purchasing behavior.
- Evaluate the clustering results using silhouette scores and visualization.

### Data

The project utilizes an Excel dataset containing transactional information about customers. Key features in the dataset include:

- CustomerID: Unique identifier for each customer.
- InvoiceDate: Date of the transaction.
- Quantity: Number of items purchased in the transaction.
- UnitPrice: Price per item.
- TotalPrice: Total revenue from the transaction.

The dataset is derived from an online retail store, containing over 390,000 rows of transaction data. Each transaction represents a purchase made by a customer on a particular date.

### Problem Statement

Understanding customer behaviors and purchasing patterns is essential for developing targeted marketing strategies and improving customer retention. The goal was to analyze online retail data to identify key customer segments and actionable patterns.

### Solution Approach

1. Data Cleaning:
- Removed rows with missing CustomerID values and filled missing Description values.
- Removed rows with negative Quantity and UnitPrice values.
- Created a new column TotalPrice by multiplying Quantity and UnitPrice.

2. Outlier Handling:
- Identified outliers using the 99th percentile for columns: Quantity, UnitPrice, and TotalPrice.
- Capped the outliers by replacing extreme values with the 99th percentile values to reduce their effect on the analysis.

3. Feature Engineering:
- Extracted new features from the InvoiceDate, including InvoiceMonth, InvoiceDayOfWeek, and InvoiceHour.
- Conducted Recency, Frequency, and Monetary (RFM) analysis for customer segmentation.

4. Exploratory Data Analysis (EDA):
- Analyzed the distribution of total revenue and order value.
- Summarized key metrics such as total revenue, average revenue, number of unique customers, and order frequency.

5. Clustering:
- KMeans Clustering: Performed KMeans clustering with varying values of k (number of clusters), using the Elbow Method to determine the optimal k.
- Hierarchical Clustering: Used Agglomerative Clustering and visualized results using a dendrogram.

6. Model Evaluation:
- Evaluated the quality of the KMeans clustering using the silhouette score. The silhouette score for k=4 was found to be 0.60, indicating a reasonably good clustering structure.  

### Visualizations

- Distribution of Total Revenue: A histogram showing the distribution of revenue per transaction.
- Customer Segmentation by Spending: Bar chart categorizing customers into Low, Medium, High, and Very High spending groups.
- Seasonal Purchase Trends: Line chart displaying monthly revenue trends for high-value customers.
- Top Products for High-Value Customers: Bar chart showing the top 10 products purchased by high-value customers.
  
### Results

- Total Revenue: 7,520,671.07
- Average Revenue: 19.15 per transaction
- Average Order Value: 405.82
- Number of Unique Customers: 4,338
- Average Order Frequency per Customer: 4.27
- Silhouette Score for k=4: 0.60

### Future Work

Further exploration could involve:

1. Fine-tune the clustering process by experimenting with different methods of outlier handling and scaling techniques.

2. Test different clustering algorithms (DBSCAN, Gaussian Mixture Models) to compare clustering results.

3. Implement additional analyses such as predictive modeling for customer churn or sales forecasting.

### Source

https://www.kaggle.com/datasets/shreyanshverma27/online-sales-dataset-popular-marketplace-data
