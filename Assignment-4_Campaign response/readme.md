# Campaign response
[![](https://img.shields.io/badge/-Python-yellow)](https://www.python.org/)

## Notebook
[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/NittyNice/BADS7105-CRM-Analytics/blob/main/Assignment-4_Campaign%20response/Campaign_response_model.ipynb) 

## Dataset
[Retail_Data_Response.csv](https://github.com/NittyNice/BADS7105-CRM-Analytics/blob/main/data/Retail_Data_Response.csv) is a dataset about responses to campaigns of individual customer.  
[Retail_Data_Transactions.csv](https://github.com/NittyNice/BADS7105-CRM-Analytics/blob/main/data/Retail_Data_Transactions.csv) is a dataset about transaction of individual customer include date and transaction amount.

## Process Overview

## Feature Engineering
We create features based on 2 well known analysis techniques.:
1) CLV (Customer Lifetime Value)
2) RFM (Recency, Frequency, and Monetary value)

### Visualize Response Distribution
First, we take a look at amount of customer who response and non-response to campaign.
![response_distribution.png](./img/response_distribution.png)

### Visualize the correlation between each pair of variables
Next, we create features based on 2 well known analysis techniques.
1) CLV  
![clv_frequency_aou.png](./img/clv_frequency_aou.png) ![clv_frequency_monetary.png](./img/clv_frequency_monetary.png) 
![clv_frequency_ticketsize.png](./img/clv_frequency_ticketsize.png) ![clv_monetary_aou.png](./img/clv_monetary_aou.png) 
![clv_monetary_ticketsize.png](./img/clv_monetary_ticketsize.png) ![clv_aou_ticketsize.png](./img/clv_aou_ticketsize.png) 
![clv_recency_aou.png](./img/clv_recency_aou.png) ![clv_recency_frequency.png](./img/clv_recency_frequency.png) 
![clv_recency_monetary.png](./img/clv_recency_monetary.png) ![clv_recency_ticketsize.png](./img/clv_recency_ticketsize.png)

1) RFM  
![overview](./img/rfm_frequency_monetary.png) ![overview](./img/rfm_recency_frequency.png) 
![overview](./img/rfm_recency_monetary.png)

### Deal with imbalanced data and split train/test
Lastly, we fixed imbalanced with SMOTE and split data to train set and test set with a ratio of 70/30.

## Classification Model
### Model 1 : Logistic Regression
1) CLV  
![logistic_regression_clv_score.png](./img/logistic_regression_clv_score.png)

- Evaluation  
![logistic_regression_clv_auc.png](./img/logistic_regression_clv_auc.png)

2) RFM  
![logistic_regression_clv_score.png](./img/logistic_regression_RFM_score.png)

- Evaluation  
![logistic_regression_clv_auc.png](./img/logistic_regression_RFM_auc.png)

### Model 2 : XGBoost
1) CLV  
![xgboost_clv_score.png](./img/xgboost_clv_score.png)

- Evaluation  
![xgboost_clv_auc.png](./img/xgboost_clv_auc.png)

- Visualize classification tree  
![xgboost_clv_tree.png](./img/xgboost_clv_tree.png)

2) RFM  
![xgboost_RFM_score.png](./img/xgboost_RFM_score.png)

- Evaluation  
![xgboost_RFM_auc.png](./img/xgboost_RFM_auc.png)

- Visualize classification tree  
![xgboost_RFM_tree.png](./img/xgboost_RFM_tree.png)

