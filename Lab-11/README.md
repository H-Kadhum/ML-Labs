# Credit Card Customer Segmentation Project

This project uses credit card customer data to group similar customers together.

## Overview

The project uses K-Means clustering to find customer groups based on their credit card behavior.

## Dataset

The dataset includes customer information such as balance, purchases, payments, cash advances, and credit limit.

## Main steps

1. Load the dataset
2. Clean the data
3. Remove the `CUST_ID` column
4. Fill missing values
5. Scale the data
6. Apply K-Means clustering
7. Choose the best number of clusters
8. Study the final customer groups

## Final result

The best number of clusters was 3.  
This means the customers were divided into 3 different segments.

## Questions and Answers

### 1. Why is this an unsupervised learning problem?

It is unsupervised because there is no target column. The model groups customers by finding patterns in the data.

### 2. Why did we remove the `CUST_ID` column?

`CUST_ID` was removed because it is only an ID number. It does not give useful information about customer behavior.

### 3. Which columns had missing values?

The missing values were found in:

- `CREDIT_LIMIT`
- `MINIMUM_PAYMENTS`

### 4. How were missing values handled?

The missing values were replaced with the mean of each column.

### 5. Why is scaling important?

Scaling is important because K-Means depends on distance. Scaling makes all columns have a similar range, so no column unfairly affects the clustering.

### 6. Which K value was chosen?

The chosen value was `K = 3`.

The elbow method showed that 3 clusters was a good point where the improvement started to slow down. The silhouette score also supported choosing 3 clusters.

### 7. What does each cluster mean?

- **Cluster 0:** Customers who use cash advance more and have higher balances.
- **Cluster 1:** Customers who spend more, pay more, and have higher credit limits.
- **Cluster 2:** Customers who use the card less and have lower activity.

### 8. Which cluster is high-value?

Cluster 1 is likely the high-value customer group because they spend more and have higher credit limits.

### 9. Which cluster depends more on cash advance?

Cluster 0 depends more on cash advance because it has the highest cash advance behavior.

### 10. How can companies use these clusters?

Companies can use these groups to make better marketing plans. They can give rewards to high-value customers, support cash advance users with better payment options, and encourage less active customers with offers.

## Libraries used

- Pandas
- Matplotlib
- Seaborn
- Scikit-learn