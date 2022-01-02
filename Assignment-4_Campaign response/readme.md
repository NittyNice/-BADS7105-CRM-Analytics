# Campaign response
[![](https://img.shields.io/badge/-Python-yellow)](https://www.python.org/)

## Notebook
[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/NittyNice/BADS7105-CRM-Analytics/blob/main/Assignment-4_Campaign%20response/Campaign_response_model.ipynb) 

## Dataset
[Retail_Data_Response.csv](https://github.com/NittyNice/BADS7105-CRM-Analytics/blob/main/data/Retail_Data_Response.csv) is a dataset about responses to campaigns of individual customer.  
[Retail_Data_Transactions.csv](https://github.com/NittyNice/BADS7105-CRM-Analytics/blob/main/data/Retail_Data_Transactions.csv) is a dataset about transaction of individual customer include date and transaction amount.

## Process Overview

## Feature Engineering
We create features based on 2 analysis technique:
1) CLV (Customer Lifetime Value)
2) RFM (Recency, Frequency, and Monetary value)

### Visualize the correlation between each pair of variables
1) CLV  
![overview](./img/clv_frequency_aou.png) ![overview](./img/clv_frequency_monetary.png) 
![overview](./img/clv_frequency_ticketsize.png) ![overview](./img/clv_monetary_aou.png) 
![overview](./img/clv_monetary_ticketsize.png) ![overview](./img/clv_aou_ticketsize.png) 
![overview](./img/clv_recency_aou.png) ![overview](./img/clv_recency_frequency.png) 
![overview](./img/clv_recency_monetary.png) ![overview](./img/clv_recency_ticketsize.png)

1) RFM  
![overview](./img/rfm_frequency_monetary) ![overview](./img/rfm_recency_frequency.png) 
![overview](./img/rfm_recency_monetary.png)

