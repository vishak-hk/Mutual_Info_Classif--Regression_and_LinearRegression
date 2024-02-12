# Part 1: Mutual Information Classification - Model Based Feature Selection

## Objective:
Perform model-based feature selection using Mutual Information Classification on the "loan" dataset.

### Steps:
1. **Load Dataset:**
   - Utilize the pandas library to load the "loan" dataset.

2. **Data Processing:**
   - Apply necessary processing, including label encoding and handling null values.

3. **Separate Features and Target:**
   - Separate features (X) and the target variable (y: Loan_Status) from the dataset.

4. **Feature Selection:**
   - Use SelectKBest from sklearn.feature_selection to select the top K features based on mutual information scores.
   - Choose an appropriate value of K.

5. **Fit and Transform:**
   - Fit the feature selection model on the dataset.
   - Transform the feature matrix accordingly.

6. **Print Selected Features:**
   - Print the names or indices of the selected features.

# Part 2: Mutual Information Regression - Model Based Feature Selection

## Objective:
Perform model-based feature selection using Mutual Information Regression on the "Housing.csv" dataset.

### Steps:
1. **Load Dataset:**
   - Load the "Housing.csv" dataset using the pandas library.

2. **Data Processing:**
   - Apply necessary processing, including label encoding and handling null values.

3. **Separate Features and Target:**
   - Separate features (X) and the target variable (y: Price of the house) from the dataset.

4. **Feature Selection:**
   - Use SelectKBest from sklearn.feature_selection to select the top K features based on mutual information scores.
   - Choose an appropriate value of K.

5. **Fit and Transform:**
   - Fit the feature selection model on the dataset.
   - Transform the feature matrix accordingly.

6. **Print Selected Features:**
   - Print the names or indices of the selected features.

# Part 3: Linear Regression on the Housing Dataset

## Objective:
Perform linear regression on the Housing dataset to predict house prices.

### Steps:
1. **Load Dataset:**
   - Load the "Housing.csv" dataset using the pandas library.

2. **Data Preprocessing:**
   - Apply necessary preprocessing steps, including handling missing values and feature scaling if required.

3. **Separate Features and Target:**
   - Separate features (X) and the target variable (y: house prices) from the dataset.

4. **Split Dataset:**
   - Split the dataset into training and testing sets using an 80:20 ratio.

5. **Feature Selection:**
   - Perform feature selection using Mutual Information Regression.
   - Select the top 30 features based on mutual information scores.

6. **Linear Regression Model:**
   - Fit a linear regression model to the training data using LinearRegression from sklearn.linear_model.

7. **Prediction:**
   - Predict house prices for the testing data using the trained model.

8. **Model Evaluation:**
   - Evaluate the model's performance using the following metrics:
     - Mean Squared Error (MSE)
     - Root Mean Squared Error (RMSE)
     - Coefficient of Determination (R^2)

9. **Print Metrics:**
   - Print the MSE, RMSE, and R^2 values to assess the model's accuracy.

10. **Scatter Plot:**
    - Plot a scatter plot between predicted and actual house prices for the testing data using matplotlib.

11. **Summary: Linear Regression Model Evaluation**
   - **Mean Squared Error (MSE):** 0.05
     - The average squared difference between predicted and actual values is 0.05. Lower MSE values indicate better model performance.
   - **Root Mean Squared Error (RMSE):** 0.22
     - The square root of the MSE, representing the average magnitude of errors in the predicted values. In this case, the RMSE is 0.22.
   - **R^2 Score:** 0.83
     - The coefficient of determination, indicating the proportion of the variance in the dependent variable that is predictable from the independent variable. An R^2 score of 0.83 suggests that the model explains 83% of the variance in the target variable.
   - **Summary:** The Linear Regression model appears to perform well, with a relatively low mean squared error and root mean squared error. The R^2 score indicates a high level of explanatory power, suggesting that the model captures a significant portion of the variance in the target variable. This indicates good predictive performance, but further analysis and consideration of specific use case requirements are advisable.
