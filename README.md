# Project: Stroke Prediction using Logistic Regression

This is a R group project for the UBC course Advanced Predictive Business Analytics. I coworked with Rhea Gupta and Kook Han for this project during January to February 2022.

### Introduction:
Our project purpose is first to examine the relationship between stroke and other predictors, and then build a valid logistic regression model to predict the probability of stroke with the selected predictor variable(s).

### Analysis Steps Breakdown:
The Rmd file contains below steps and related analysis. You can execute the whole RMD file to generate statistics results.

Step 1. Report Summary Statistics after Data Cleansing

Step 2. Assess Model Assumptions including Linearity, Additivity, and Multicollinearity

Step 3. Variable Selections using Stepwise Backward Selection

Step 4. Modelling with and without influential observations

Step 5. Working Model Interperatation: Log-odds and corresponding odd ratios, R2, LR test, Discrimination Indexes
<p align = 'center'>
<img src = 'https://github.com/vivianddyu/LogisticRegression/blob/main/Age_on_Stroke_by_Hypertension.PNG?raw=true'>
</p>

Step 6. Model Validation: Shrinkage, Calibration, and Bootstrap Validation
We take an additional step to adjust the effects of using stepwise backward variable selection.

Step 7. Comparison with an alternative model built with Principle Component Analysis: AIC, and model statistics

### Results:
Our final model has two predictor variables Age and Hypertension, and can account for 27.8% of variations in the outcomes. According to our final model, there's a 282% increase in the odds of the outcome (stroke) for a person with hypertension compared with a person without hypertension, while everything else remains the same. There's a 7% increase in the odds of the outcome (stroke) for a 1-year increase in age, while controlling all other attributes.
In conclusion, overall our model performs well: (1) Shrinkage is around 97%, indicating a good performance when deploying this model to other datasets. (2) Calibration of our model is good as the model's predictions are close to those of an ideal model . (3) Our model also outperforms alternative PCA model in almost every aspect including R2, discrimination, and AIC.
