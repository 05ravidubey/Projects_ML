# Advertising Sales Prediction using Linear & Ridge Regression

##  Objective
Predict product sales based on advertising spend across TV, Radio, and Newspaper channels.

##  Dataset
Source: Kaggle / Advertising dataset
  Features:
  TV
  Radio
  Newspaper
  Target:
  Sales

## Project Workflow
1. Data Cleaning
2. Exploratory Data Analysis (EDA)- Linerity and Multicolnearity checked
3. Feature Engineering- Winsorisation and log transformation done on newspaper col.
4. Train-Test Split
5. Feature Scaling
6. Model Training:
   - Linear Regression
   - Ridge Regression
   - Lasso Regression
7. Cross Validation
8. Model Evaluation
9. Without  newspapers columns
    

---

## Models Used

## Linear Regression
Baseline model

## Ridge Regression
Used to handle multicollinearity
Improves model stability

## Evaluation Metrics

 Metric - Value 
 Model       MAE      RMSE        R2
0  Linear  1.463402  1.776717  0.899988
1   Ridge  1.465326  1.780978  0.899508
2   Lasso  1.461653  1.791383  0.898331

## Cross Validation
5-Fold CV used
CV Linear: 0.8877746326163092
CV Ridge: 0.8877747532220847
CV Lasso: 0.8877776446006129

## Key Insights
- TV and Radio strongly impact sales
- Newspaper has weak correlation
  Model is not overfit.
- without news paper col also models R2 score was same

