# AB testing
 [![](https://img.shields.io/badge/-Analysis--toolpak-green)](https://support.microsoft.com/en-us/office/load-the-analysis-toolpak-in-excel-6a63e598-cd6d-42e3-9317-6b40ba1a66b4)
 [![](https://img.shields.io/badge/-Excel-green)](https://www.microsoft.com/en-us/microsoft-365/excel)
 
## Dataset
[AB testing survey](https://github.com/NittyNice/BADS7105-CRM-Analytics/blob/main/data/AB%20Testing%20Survey.csv) is a preference questionnaire between warm and cool colored pens. The survey required gender, age, purpose of pen and satisfy score of different colored pen.
- Gender : Male, Female
- Age : Integer
- Purpose : Study, Work
- Satisfaction Score of each pen : 1 - 5 (5 = Very satisfied)
 
## Survey
The objective of the AB test is to choose a pen color, turquoise and orange, to give an attendees.  

![](./img/pen_turquoise.png) ![](./img/pen_orange.png)
 
## Exploratory Data Analysis
Take a look at the proportion between men and women and the proportion of the purpose of use.  
There are 50 respondents.  
Geder  
Male: 32  
Female: = 18  

The purpose of pen  
For work: 32  
For study: 18  

![](./img/gender.png) ![](./img/purpose.png)
 
Next, look at the mean and variance of satisfaction scores.  

![](./img/summarize.png)
 
## Hypothesis Testing overall  
#### satisfy score distribuion  
![](./img/score_of_turquoise_pen.png) ![](./img/score_of_orange_pen.png)

#### T-Test
![](./img/t_test_all.png)


## Hypothesis Testing Gender Effect
#### satisfy score distribuion  
![](./img/score_of_turquoise_pen_man.png) ![](./img/score_of_orange_pen_man.png) 
![](./img/score_of_turquoise_pen_woman.png) ![](./img/score_of_orange_pen_woman.png)

#### T-Test
![](./img/t_test_gender.png)



## Hypothesis Testing Purpose Effect  
#### satisfy score distribuion  
![](./img/score_of_turquoise_pen_for_study.png) ![](./img/score_of_orange_pen_for_study.png) 
![](./img/score_of_turquoise_pen_for_work.png) ![](./img/score_of_orange_pen_for_work.png)

#### T-Test
![](./img/t_test_purpose.png)
 
