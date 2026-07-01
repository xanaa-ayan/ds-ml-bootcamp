# Part C — Reflection Paper 

---

### 1. What did you implement?
In this assignment, I successfully implemented a supervised machine learning regression pipeline to predict car prices. Using the cleaned car dataset from Assignment Three, I defined the input attributes as features ($X$) and the car price as the continuous output label ($y$). I split the dataset into an 80% training set and a 20% testing set to ensure unbiased evaluation. I then trained two distinct regression models: a basic Linear Regression model and a more complex Random Forest Regressor.

### 2. Comparison of Models & Sanity Check
During the sanity check on a single test observation, the model predictions displayed visible differences. The Linear Regression model provided a projection based entirely on rigid linear patterns, which sometimes resulted in unrealistic values when certain attributes shifted. On the other hand, the Random Forest Regressor produced a prediction much closer to the average surrounding actual prices. Random Forest yielded more realistic outcomes because it captures non-linear complexities and limits the impact of unexpected feature combinations.

### 3. Understanding Random Forest
In my own words, Random Forest is an ensemble machine learning algorithm used for both classification and regression. Instead of relying on a single Decision Tree (which is highly prone to overfitting), Random Forest builds a "forest" of multiple decision trees on randomly selected subsets of the data and features. During inference, each tree casts its own independent prediction, and the final output is determined by taking the mathematical average of all predictions. This collaborative framework reduces variance and improves overall model accuracy.

### 4. Metrics Discussion
Based on the experiment metrics:
* The Random Forest model achieved a significantly lower Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) compared to the Linear Regression model.
* The $R^2$ score for Random Forest was substantially higher, indicating that it explained a much larger percentage of the variance in used car pricing.
This tells us that Linear Regression is limited when handling data where features interact in complex, non-linear ways (e.g., how age and mileage combined impact a vehicle's depreciation). Random Forest is highly robust against non-linear interactions, making it vastly superior for real-world messy asset pricing.

### 5. Final Findings & Model Preference
In conclusion, I firmly prefer the **Random Forest Regressor** for predicting car prices in this project. Real-world car markets do not follow a simple straight-line depreciation; a luxury car might lose value differently than a standard commercial vehicle, and age affects value exponentially rather than linearly. 

Random Forest handles these nuances perfectly without needing complex mathematical transformations beforehand. It delivers lower errors, minimizes the danger of outlier distortion, and maximizes predictive accuracy, making it the ideal choice for deployment in a production data science lifecycle.