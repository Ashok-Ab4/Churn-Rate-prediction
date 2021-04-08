# Churn-Rate-prediction


#### Point of the project is to predict if a customer will Churn (Leave the service) 

#### In the first notebook 'Data Cleaning' we go through the dataset and perform several data cleanup steps - null handling, correlation of features, dummy encoding categorical variables and then save the resulting dataset as a csv file. 

#### In the second notebook 'Churn Rate Prediction - Model Building' we first load in the cleaned dataset. Then to handle class imbalance we up sample the minority class in the predictor variable using SMOTE (Synthetic Minority Oversampling Technique). Once the classes are balanced the dataset is fed into a pipeline with 4 classifiers - KNN, Logistic Regression, Decision Tree and Random Forest Classifiers. The best performing model then subjected to hyperparameter tuning, and RF ended up being the best performing model overall. But due to the high number of False negatives, the model with the lease number of false negatives was chosen as the final model (Logistic Regression). 

#### Hyperparameter tuning then performed on logistic regression, Then AOC plots gerenated for all models and calculations made to see what the optimal thresholds are for all the models. 

#### Finally cost evaluations are performed with the different scenarios to see what scenario would ensure least amount of customers churning and minimising the costs incurred.
