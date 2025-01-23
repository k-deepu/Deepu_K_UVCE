# Deepu_K_UVCE
This project aims to segment customers into distinct groups based on their profile information and transaction behavior using clustering techniques. The goal is to identify patterns in customer spending and demographics, enabling businesses to tailor their marketing strategies and improve customer engagement.

Datasets
Customers.csv: Contains demographic details of customers, such as CustomerID, CustomerName, Region, and SignupDate.
Transactions.csv: Contains transactional data, including TransactionID, CustomerID, ProductID, TransactionDate, Quantity, TotalValue, and Price.
Approach
Data Merging and Preprocessing:

We merged the Customers.csv and Transactions.csv datasets based on CustomerID.
Aggregated the transaction data for each customer: total spending (TotalValue), total quantity purchased (Quantity), and frequency of transactions (TransactionCount).
One-hot encoded the Region column to convert categorical data into numerical format.
Converted the SignupDate into a numerical feature representing the number of days since signup.
Feature Engineering:

Profile Features: Region (one-hot encoded), SignupDate (days since signup).
Transaction Features: TotalValue, Quantity, and TransactionCount.
Clustering with K-Means:

Applied K-Means clustering to segment customers based on the engineered features.
Standardized the features using StandardScaler to ensure equal contribution from each feature.
Chose 4 clusters for the segmentation.
Clustering Evaluation:

Davies-Bouldin Index (DB Index) was used to evaluate the clustering quality. A lower DB Index indicates better clustering.
Visualization:

A scatter plot was generated to visualize the customer clusters based on TotalValue and Quantity.
Results
Number of Clusters: 4 clusters were identified based on customer behavior.
DB Index: The DB Index value was calculated to assess the quality of the clustering.
Clustering Visualization: A scatter plot shows how customers are grouped based on their transaction behavior and profile features.
Requirements
Python 3.x
pandas
numpy
scikit-learn
matplotlib
