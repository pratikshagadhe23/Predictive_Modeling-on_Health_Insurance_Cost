# Predictive Modeling on Health Insurance Cost

This project aims to build predictive models to estimate health insurance charges based on various personal attributes. The dataset, sourced from Kaggle, includes variables such as age, sex, BMI, smoking status, region, and number of children. Several regression models were evaluated to identify the best predictors for insurance costs.

## Table of Contents

1. [Introduction](#introduction)
2. [Objectives](#objectives)
3. [Data Exploration](#data-exploration)
4. [Modeling](#modeling)
    - [Multiple Linear Regression](#multiple-linear-regression)
    - [LASSO Regression](#lasso-regression)
    - [Decision Tree](#decision-tree)
    - [Random Forest](#random-forest)
    - [Bagging](#bagging)
    - [Gradient Boosting](#gradient-boosting)
5. [Model Evaluations](#model-evaluations)
6. [Conclusion](#conclusion)
7. [References](#references)
8. [Code Appendix](#code-appendix)

## Introduction

The rising cost of healthcare in the United States has created a significant burden on families, businesses, and taxpayers. This project explores the factors contributing to these high costs and aims to develop predictive models to estimate health insurance charges.

## Objectives

- To find the best regression model
- To predict health insurance charges based on personal data

## Data Exploration

- **Data Source**: The dataset was obtained from Kaggle and focuses on the USA region with 1338 observations and 7 variables.
- **Data Pre-processing**: No missing data points were identified.
- **Exploratory Data Analysis**: Summary statistics and data visualizations were generated to understand the relationships between variables.

## Modeling

### Multiple Linear Regression

Initial models did not satisfy assumptions of linearity, constant variance, and normality. A final model was chosen based on the least Akaike Information Criterion (AIC) value.

### LASSO Regression

Used L1 regularization to avoid overfitting. Important variables identified were smoker, age, and BMI.

### Decision Tree

Built using binary splits to minimize a cost function. Important variables were smoker, age, and BMI.

### Random Forest

An ensemble of decision trees that aggregated results. Important variables identified were smoker, age, and BMI.

### Bagging

Built multiple decision trees using bootstrapping. Important variables identified were age, BMI, and smoker.

### Gradient Boosting

An ensemble method that builds decision trees by reducing the loss function. Important variables identified were smoker, age, and BMI.

## Model Evaluations

- Models were evaluated using Root Mean Squared Error (RMSE).
- The model with the least RMSE value of about 4480.7 was identified as the best performer.

## Conclusion

- **Findings**: Age, BMI, and smoking status are crucial predictors of health insurance charges.
- **Limitations**: The data is confined to the US region and might be biased due to unbalanced factor levels.
- **Future Ideas**: Consider additional variables and collect more data for improved predictions.

## References

- [ResearchGate on Akaike Information Criterion](https://www.researchgate.net/post/Akaike_information_criterion#:~:text=But%20to%20answer%20your%20question,above%20answer%2C%20comparing%20AICs)
- [Modern Data Science with R](https://mdsr-book.github.io/mdsr2e/ch-learningI.html#sec:tuning)
- [Kaggle Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)

## Code Appendix

- [GitHub Repository](https://github.com/pratikshagadhe23/Predictive_Modeling-on_Health_Insurance_Cost)
