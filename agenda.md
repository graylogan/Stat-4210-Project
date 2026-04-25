# TO-DO

## Roles
* Person A: Renovation Need Classification 
* Person B: Linear Model, Regularization, and  non-linear for sale price
* Person C: Dataset summary stats; Tree based models and Deep learning for sale price
* Person D: Renovation Impact, Temporal Trends, Unsupervised Learning

## Summary Statistics
* How many observations?
* Summary statistics for most relevant predictors:
  * mean
  * std dev
  * percentiles
  * min/max

## Sale Price Prediction
### Baseline Models
* Linear Regression
### Regularization / Shrinkage
* Ridge Regression
* LASSO
### Nonlinear Regression
* Splines
* LOESS (Local Regression)
* Generalized Additive Models (GAMs)
### Tree-Based Models
* Decision Trees
* Random Forests (Bagging)
* Boosting
### Deep Learning
* Neural Network regression model
### Evaluation
* RMSE
* MSE
* R²
* Cross-validation / validation set

## Renovation Need Classification
Classify all homes with overal condition < 5/10 as in need of renovation. Then, train classifiers on labeled data.
### Classification Models
* Logistic Regression
* K-Nearest Neighbors (KNN)
* Linear Discriminant Analysis (LDA)
* Quadratic Discriminant Analysis (QDA)
* Support Vector Machine (SVM)
* Neural Network classifier
### Evaluation
* Accuracy
* Recall
* Confusion Matrix

# Renovation Impact Analysis
Create feature that represents the years since the home was rennovated. Fit a linear model for sale price including this predictor. The rennovation coefficient represents how much on average each year since rennovation decreases the home price by.

# Temporal Trend Analysis
* Similar to rennovation impact
* Create categorical year variables (allows us to capture 2008 housing crash?)
* Create categorical season variables for trends throughout year
* Look at coefficients
* Can include box plots for sale price by month

# Unsupervised Learning
* K-Means clustering
* Summarize each cluster with statistics (mean, std dev, quartiles, etc.)
* Identify clusters such as:
  * high-end homes
  * mid-range homes
  * budget homes

# Model Comparison
* RMSE / MSE
* R²
* Cross-validation performance
* Bias–variance considerations
* Interpretability
* Model complexity