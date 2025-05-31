# Predicting Term Deposit Subscriptions with ROC-Optimized Machine Learning Models

## Project Summary
This project develops a predictive machine learning model to support targeted marketing strategies for a Portuguese banking institution. Using customer data collected from past marketing campaigns, the goal is to identify the likelihood that a customer will subscribe to a term deposit.

To align with the business objective of maximizing conversions, the focus was placed on ranking models by their ability to distinguish between positive and negative outcomes. Therefore, the models were evaluated using the ROC AUC metric, which reflects the model’s capability to prioritize customers most likely to subscribe.

Four classification algorithms were explored:
	•	Logistic Regression
	•	K-Nearest Neighbors (KNN)
	•	Decision Tree Classifier
	•	Support Vector Machine (SVM)

Each model was fine-tuned using GridSearchCV and validated with cross-validation. Data preprocessing steps included one-hot encoding for categorical variables and standardization where necessary. The final models were compared based on ROC AUC scores, and ROC curves were plotted for visual comparison.

The project follows a CRISP-DM-like process and is designed to inform marketing strategies by helping the business focus its efforts on the customers most likely to convert.

## Notebook
👉 [Click here to view the full Jupyter notebook](https://github.com/AriAlas/ml-comparing-classifiers/blob/main/comparing-classifiers.ipynb)

## Model Evaluation & Business Insights


## Key Insights
