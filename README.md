# Customer-Lifetime-Value

### Summary and Recommendations

#### 1. Overview

The project involves using historical sales data to predict future customer value. By calculating RFM (Recency, Frequency, Monetary) metrics, the code builds models to predict CLV and then segments customers based on their predicted value into **Low**, **Medium**, and **High CLV** groups. 

#### 2. Data

The project utilizes an Excel dataset containing transactional information about customers. Key features in the dataset include:

- CustomerID: Unique identifier for each customer.
- InvoiceDate: Date of the transaction.
- Quantity: Number of items purchased in the transaction.
- UnitPrice: Price per item.
- TotalPrice: Total revenue from the transaction.

The dataset is derived from an online retail store, containing over 390,000 rows of transaction data. Each transaction represents a purchase made by a customer on a particular date.

#### 3. Method

1. Data Cleaning
2. Feature Engineering
3. Exploratory Data Analysis (EDA)
4. Customer Segmentation:
- Utilize K-Means and Hierarchical Clustering to segment customers based on RFM metrics.
- Calculate the Silhouette Score to evaluate the quality of clustering.
7. Modeling
8. Customer Segmentation Based on Predicted CLV
  
#### 4. Key Findings

- Total Revenue: 8,887,208.89
- Average Revenue per Transaction: 22.63Average Order Value (AOV): 479.56
- Number of Unique Customers: 4,338
- Average Order Frequency per Customer: 4.27
- The clustering analysis helps to identify high-value customers and tailor marketing strategies accordingly.
- The regression models provide valuable predictions of CLV, aiding in better customer relationship management.

#### 5. Future Work

Further exploration could involve:

- Implementing more advanced predictive modeling techniques.
- Incorporating additional customer features (e.g., demographic data).
- Conducting a deeper analysis of customer segments to improve targeting strategies.

#### 6. Source

https://www.kaggle.com/datasets/shreyanshverma27/online-sales-dataset-popular-marketplace-data
