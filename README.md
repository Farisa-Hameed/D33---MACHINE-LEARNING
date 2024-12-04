# D33---MACHINE-LEARNING
1. Loading and Preprocessing
   
In the first step, we loaded the dataset and performed initial exploration using methods like .head(), .info(), and .describe() to inspect the structure and identify any missing values. We handled missing data by dropping rows with null values and encoded categorical variables using one-hot encoding to prepare them for machine learning models. Numerical features were scaled using StandardScaler to standardize the data, ensuring all features were on the same scale. Finally, the data was split into training and testing sets using train_test_split for model training and evaluation.

2. Model Implementation
   
We implemented five regression algorithms: Linear Regression, Decision Tree Regressor, Random Forest Regressor, Gradient Boosting Regressor, and Support Vector Regressor. Each model was trained using the training set and evaluated using the test set. We calculated performance metrics including R-squared, Mean Squared Error (MSE), and Mean Absolute Error (MAE) to assess how well each model predicted car prices. The results showed varying levels of model accuracy, which allowed us to compare and select the best-performing model.

3. Model Evaluation

The performance of each model was compared using three evaluation metrics: R-squared, MSE, and MAE. These metrics helped determine the model that best predicted car prices. The Random Forest Regressor performed the best in terms of R-squared and other metrics, indicating that it was the most accurate model for this dataset. A bar plot was used to visualize the performance of all models, highlighting the differences in their ability to capture the variability in car prices.

4. Feature Importance Analysis
   
After identifying the best model (Random Forest Regressor), we analyzed the feature importance to determine which variables had the greatest impact on car prices. Random Forest provided feature importance scores, which we visualized using a bar plot. This analysis helped identify the most influential features in the dataset, such as engine size, fuel efficiency, and vehicle age, which could guide business decisions related to car pricing strategies.

5. Hyperparameter Tuning
   
Hyperparameter tuning was performed for the Random Forest Regressor using GridSearchCV to optimize parameters like the number of estimators, maximum depth, and minimum samples per split. After tuning, the model’s performance was evaluated again, showing slight improvements in accuracy (R-squared) and error metrics (MSE and MAE). This confirmed that hyperparameter tuning enhanced the model’s predictive power, allowing it to better capture the relationships between features and car prices.

6. Submission
    
The entire process, including model implementation, evaluation, feature importance analysis, and hyperparameter tuning, was documented in a Jupyter notebook. The notebook was thoroughly commented and explained, making it easy to understand the workflow and results. The final version of the notebook was saved and uploaded to GitHub for submission, fulfilling the requirements of the assignment.
