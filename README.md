# Online-Retail-Customer-Segmentation
#### Unsupervised - Machine Learning Algorithm

## Business Objective
In this project, our task is to identify customer segments on a transnational dataset which contains all transactions between 01/12/2010 and 09/12/2011 for a UK based and registered non-store online retail. The company sells gift items and the buyers are mostly wholesellers.

## Why divide Customers into Clusters?
Clustering helps to make a group with similar characteristics. With the help of clustering, we can divide cutomers into groups with similar features and thus apply different marketing techniques, different promotional offers for separate groups. 

## Dataset Overview
The dataset consists of 5,41,909 rows and 8 columns. The columns are InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country. The columns have both numerical and categorical data types. There are 5268 rows with duplicate values. Whereas, 135080 CustomerID's are null and 1454 Description's are null. 

## Dataset PreProcessing
Removed all the duplicate rows. Also, if the InvoiceNo contains a letter C then it means that it is a cancellation order. So, removed those records as well. Additionally, if the Quantity has negative values, it means that those are cancelled records, so removed those records as well. 

## Exploratory Data Analysis
Some important findings from EDA are:
- Most of the customers are based in United Kingdom, with the next highest coming from Germany and France.
- WHITE HANGING HEART T-LIGHT HOLDER is the most ordered product in terms of number of orders. PAPER CRAFT , LITTLE BIRDIE is the most ordered product in terms of quantities sold.
- CustomerID 14646.0 has spent the most amount of money.
- The month of November has highest sales followed by October.

## Feature Engineering
- Created a new column with the help of two columns.
- For modelling, we have made a RFM table. RFM stands for Recency, Frequency and Monetary. Recency is calculated as number of days since the last customer visited. Frequency is number of times customer has purchased something. Monetary is total amount that the customer has spent.
- Used Log Transformation and Cuberoot Transformation for making the features normally distributed.
- Used StandardScaler for feature scaling.

## ML Model Implementation
- K-Means Clustering with Silhouette Method
- K-Means Clustering with Elbow Method
- Hierarchical Clustering with Dendograms

## Summary
- Successfully able to divide our dataset into 3 clusters using Hierarchical Clustering because it demonstrated a better visual representation than other models.
- The project was successfully deployed thus providing a better understanding of customer preferences with targeted marketing techniques and promotional offers.
- This project will certainly help the business in customer retention, optimise pricing thus positively impacting business outcomes.
