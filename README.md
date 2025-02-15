# Churn-Prediction-Model-using-Machine-Learning
The Churn Prediction Model uses PyCaret to predict customer churn for a telecom/DTH service. By analyzing historical data, it identifies at-risk customers, aiding retention strategies. The model employs ensemble techniques for robust performance on training and testing datasets.
Introduction
This project involves developing a churn prediction model using PyCaret to identify customers at risk of leaving a telecommunication/DTH service. By analyzing historical data and relevant features, the model aims to help businesses retain customers by predicting churn likelihood.

Dataset and Problem Statement
The dataset (trainingdata.csv) includes various customer attributes and a target variable, 'status', indicating whether a customer has churned. The goal is to build a predictive model that accurately identifies customers at risk of churn based on their historical behavior and other relevant features.

Methodology
Data Preparation
Data Loading: The dataset is loaded into a Pandas DataFrame for exploration and preprocessing.
Feature Engineering: Preprocessing steps include handling missing values, encoding categorical variables, and scaling numerical features.
Model Training and Evaluation
Setup with PyCaret: The setup() function initializes the training environment, specifying the target variable and reserving data for validation.
Model Selection: The compare_models() function evaluates various machine learning models to identify top performers.
Model Blending: Top models are ensembled using blend_models() to create a final blended model, enhancing predictive performance.
Model Evaluation
Evaluation Metrics: Metrics such as accuracy, precision, recall, and F1-score are computed to assess model performance.
Confusion Matrix: A confusion matrix provides a detailed view of true positives, true negatives, false positives, and false negatives.
Graph: A graph is plotted between actual and predicted values using the Plotly library.
Manual Testing
New Data for Manual Testing: A sample of new data is created to simulate real-time predictions.
Prediction on New Data: The final blended model predicts churn probability for new data, converting predictions into binary outcomes.
Prediction on Given Data
Prediction on Training Data: The model predicts churn probabilities on the original training dataset to validate performance.
Predicting on Testing Data
Loading and Predicting on Testing Data: The final model predicts churn probabilities on a separate testing dataset, converting predictions into binary outcomes.
Results and Discussion
Model Performance: The final blended model demonstrates robust performance based on evaluation metrics, effectively identifying customers at risk of churn.
Confusion Matrix Analysis: The confusion matrix highlights areas of model strength and areas needing improvement.
Conclusion
The churn prediction model provides a systematic approach to identifying at-risk customers using historical data and relevant features. By leveraging ensemble techniques, the model achieves strong performance on both training and testing datasets. This project outlines the methodology, results, and recommendations for implementing a churn prediction model, aiding in customer retention strategies.
