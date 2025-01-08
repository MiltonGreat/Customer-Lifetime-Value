# Online Retail Data Analysis and Customer Segmentation

### Problem Statement

Understanding customer behaviors and purchasing patterns is essential for developing targeted marketing strategies and improving customer retention. The goal was to analyze online retail data to identify key customer segments and actionable patterns.

### Solution Approach

Data: Customer transaction history, purchase frequencies, and product categories.

Methods:

- Performed Recency, Frequency, Monetary (RFM) analysis to categorize customers based on purchasing behavior.
- Applied clustering techniques (K-Means) to segment customers into actionable groups, such as high-value and at-risk customers.
- Conducted trend analysis to identify seasonal purchasing behaviors.
- Tools: Python (pandas, Scikit-learn, Seaborn, Matplotlib).

### Results

- Identified three key customer segments: high-value, frequent shoppers, and one-time buyers.
- Recommended personalized email campaigns for high-value customers, resulting in a projected 15% increase in retention rates.

### Key Insights

- Targeting customers based on RFM segmentation enables more effective marketing efforts.
- Seasonal trends provide opportunities for timed promotions and campaigns.

### Overview

This project analyzes an online retail dataset to uncover customer behaviors, purchasing patterns, and revenue contributions. It employs data cleaning, exploratory data analysis (EDA), and advanced clustering techniques to segment customers based on their Recency, Frequency, and Monetary (RFM) values. The insights from this analysis provide actionable recommendations for improving customer retention, increasing revenue, and enhancing marketing strategies.

### Data

The project utilizes an Excel dataset containing transactional information about customers. Key features in the dataset include:

- CustomerID: Unique identifier for each customer.
- InvoiceDate: Date of the transaction.
- Quantity: Number of items purchased in the transaction.
- UnitPrice: Price per item.
- TotalPrice: Total revenue from the transaction.

The dataset is derived from an online retail store, containing over 390,000 rows of transaction data. Each transaction represents a purchase made by a customer on a particular date.

### Visualizations

- Distribution of Total Revenue: A histogram showing the distribution of revenue per transaction.
- Customer Segmentation by Spending: Bar chart categorizing customers into Low, Medium, High, and Very High spending groups.
- Seasonal Purchase Trends: Line chart displaying monthly revenue trends for high-value customers.
- Top Products for High-Value Customers: Bar chart showing the top 10 products purchased by high-value customers.
  
### Key Findings

- Total Revenue: 8,887,208.89
- Average Revenue per Transaction: 22.63Average Order Value (AOV): 479.56
- Number of Unique Customers: 4,338
- Average Order Frequency per Customer: 4.27
- The clustering analysis helps to identify high-value customers and tailor marketing strategies accordingly.
- The regression models provide valuable predictions of CLV, aiding in better customer relationship management.

### Future Work

Further exploration could involve:

- Implementing more advanced predictive modeling techniques.
- Incorporating additional customer features (e.g., demographic data).
- Conducting a deeper analysis of customer segments to improve targeting strategies.

### Source

https://www.kaggle.com/datasets/shreyanshverma27/online-sales-dataset-popular-marketplace-data
