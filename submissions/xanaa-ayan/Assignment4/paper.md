# Assignment 4: Machine Learning Modeling (Theory)
**Course:** Data Science & Machine Learning Bootcamp  
**Prepared by:** [Hanaan bashir dahir GitHub Username: xanaa-ayan]  
**Date:** July 1, 2026  

---

## Part A — Core Concepts

### 1. Linear Regression vs. Random Forest Regression
* **Linear Regression:** It is a parametric algorithm that assumes a linear relationship between the input features ($X$) and the target continuous variable ($y$). It attempts to fit a straight line (or hyperplane in multiple dimensions) that minimizes the sum of squared residuals (errors).
* **Random Forest Regressor:** It is a non-parametric, ensemble learning method that builds multiple decision trees during training. It merges their predictions (by averaging them) to get a more accurate and stable prediction. It does not assume any linear relationship and handles complex non-linear data efficiently.

### 2. Evaluation Metrics Explained
* **MAE (Mean Absolute Error):** It measures the average magnitude of errors in a set of predictions, without considering their direction. It is calculated as the average of absolute differences between actual and predicted values. It gives a direct understanding of the error in original units (e.g., USD).
* **RMSE (Root Mean Squared Error):** It is the square root of the average of squared differences between prediction and actual observation. Because it squares the errors before averaging, it gives a relatively high weight to large errors. This makes RMSE highly sensitive to outliers.
* **R² (Coefficient of Determination):** It represents the proportion of variance in the dependent variable that is predictable from the independent variables. An $R^2$ of 0.85 means 85% of the variance in car prices is explained by the model's features.

### 3. The Need for Train-Test Split
Splitting data into training and testing sets is crucial to evaluate how well the machine learning model generalizes to unseen real-world data. Training a model on the entire dataset leads to overfitting, where the model simply memorizes the noise and specifics of that data instead of learning general rules. Testing on an independent set ensures unbiased evaluation.