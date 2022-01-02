# Product Reccommendation
[![](https://img.shields.io/badge/-Python-yellow)](https://www.python.org/)

## Notebook
[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/NittyNice/BADS7105-CRM-Analytics/blob/main/Assignment-3_Product%20recommendation/Product_recommendation.ipynb) 

## Dataset
[Customet Preference Survey](https://github.com/NittyNice/BADS7105-CRM-Analytics/blob/main/data/Customer%20Preference%20Survey.csv) is survey about lists of product that asked respondents have been purchased or never purchased.


## Requirement
- [MLxtend](http://rasbt.github.io/mlxtend/) is a Python library of useful tools for the day-to-day data science tasks. 

## Process Overview

## Top 10 best sellers
There were a total of 26 products in the survey. We want to know the top 10 most popular products.  

![top_ten_selling.png](./img/top_ten_selling.png)

## Market Basket Analysis with Association Rules
### Key torms  
1) Itemset: A group of one or more products is represented by the symbol set {X} e.g. {ipad case, Refrigerator, Running shoes}.
2) Association rule: relationship rules Between the two itemset, an association rule is an implication expression of the form Itemset LHS (Left-hand side) => Itemset RHS (Right-hand side) e.g. {ipad case, Refrigerator, Running shoes} => {Musical Instruments}.

### Metrics  
Metrics for evaluating association rules and setting selection thresholds are listed below:
1) Support
h<sub>&theta;</sub>(x) = &theta;<sub>o</sub> x + &theta;<sub>1</sub>x
