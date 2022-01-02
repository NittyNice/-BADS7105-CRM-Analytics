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
The table produced by the association rule mining algorithm contains three different support metrics: 'antecedent support', 'consequent support', and 'support'. Here, 'antecedent support' computes the proportion of transactions that contain the antecedent LHS, 'consequent support' computes the support for the itemset of the consequent RHS and, 'support' computes the proportion of transactions that contain the antecedent LHS and consequent RHS otgether.  

support(LHS => RHS) = support(LHS &cup; RHS), range: [0, 1]

2) Confidence  
The confidence of a rule LHS => RHS is the probability of seeing the consequent in a transaction given that it also contains the antecedent. Note that the metric is not symmetric or directed; for instance, the confidence for LHS => RHS is different than the confidence for RHS => LHS.  
The confidence is 1 (maximal) for a rule LHS => RHS if the consequent and antecedent always occur together.

confidence(LHS => RHS) = 
![\Large x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}](https://latex.codecogs.com/svg.latex?\Large&space;x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}) 

3) Lift  
The lift metric is commonly used to measure how much more often the antecedent and consequent of a rule A->C occur together than we would expect if they were statistically independent. If A and C are independent, the Lift score will be exactly 1.



