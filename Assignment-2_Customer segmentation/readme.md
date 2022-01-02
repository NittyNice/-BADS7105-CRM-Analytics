# Customer Segmentation
[![](https://img.shields.io/badge/-Python-yellow)](https://www.python.org/)

## Notebook
[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/NittyNice/BADS7105-CRM-Analytics/blob/main/Assignment-2_Customer%20segmentation/Customer_segmentation.ipynb) 
[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/NittyNice/BADS7105-CRM-Analytics/blob/main/Assignment-2_Customer%20segmentation/Customer_segmentation_lighten.ipynb) 

## Dataset
[supermarket data](https://github.com/NittyNice/BADS7105-CRM-Analytics/blob/main/data/Supermarket%20Data.csv) is table that records each individual transaction are including basket information, customer information, product information, date, quantity, spend, and store information.  

## Requirement
- [PyCaret](https://pycaret.org/) is an open source, low-code machine learning library in Python that allows you to go from preparing your data to deploying your model within minutes.
- [Plotly](https://plotly.com/), The front end for ML and data science models.

## Process Overview

## Features Engineering
Select and calculate features for create clustering model show below:  
- `Total spend`: sum of spending
- `Total visits`: total number transactions (by count distinct BASKET ID)
- `Total SKUs`: total number of product SKUs that individual user has purchased (by count distinct PRODUCT CODE)
- `Ticket size`: average spend per transaction (by Total spend/Total visits)
- `Total days`: time period from the first transaction to the last in days
- `Recency`: duration in days from the last transaction
- `Lifetime visit frequency`: frequency of transactions per day over the lifetime relationship

## K-Means Clustering
We found that the number of customers who made only one transaction is 2,025 and the rest of 4,075 customers made at least 2 transactions.  
  
In one transaction group, certain features are available to create clustering model, becouse everyone has same value of `Total visits` and `Total days` and certain features calculate by some features with `Total visits`. Therefore, it splits into two groups and creates a specific model for each group.  

### One Time Purchase
#### Features
`Total spend` : sum of all spend.
`Total SKUs` : total of product types that customer purchased.
`Recency` : duration in days customer gone since last transaction.

#### Choosing K clusters
![](./img/onetime_kmean_select_k_metrics.png)
![](./img/onetime_kmean_plot_elbow.png)

### Many Time Purchase
#### Features
`Total spend` : sum of all spend.
`Total visits` : total number transactions.
`Total SKUs` : total of product types that customer purchased.
`Ticket size` : average spend per transaction.
`Total days`: time period of relationship.
`Recency` : duration in days customer gone since last purchased.
`Lifetime visit frequency`: frequency of transactions per day over the lifetime relationship.




