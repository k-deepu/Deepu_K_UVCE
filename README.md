# Deepu_K_UVCE

Overview
This project segments customers based on profile information and transaction data using clustering techniques. The goal is to group customers for targeted marketing strategies.

Datasets
Customers.csv: Customer demographics (CustomerID, Region, SignupDate).
Transactions.csv: Transaction data (TransactionID, CustomerID, TotalValue, Quantity).

Approach
Data Merging & Preprocessing: Merged customer and transaction data. Aggregated transaction details (total spending, quantity, frequency). One-hot encoded Region and calculated days since signup.
Clustering: Applied K-Means with 4 clusters, standardized features (TotalValue, Quantity, DaysSinceSignup).
Evaluation: Calculated Davies-Bouldin Index (DB Index) to evaluate clustering quality.
Visualization: Generated a scatter plot of TotalValue vs. Quantity with clusters.

Requirements
Python 3.x
pandas, numpy, scikit-learn, matplotlib

Deliverables
Jupyter Notebook/Python Script: Contains the code for clustering and visualization.
Clustering Report: PDF report with clustering details, DB Index, and visualizations.

Evaluation
Correct application of K-Means and evaluation metrics (DB Index).
Clear visual representation of clusters.
