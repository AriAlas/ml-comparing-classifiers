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
To evaluate model performance, ROC AUC was used as the primery metric, aligning with the goal of prioritizing customers most likely to subscribe to a term deposit. Below is a summary of findings from the final model comparison:


[paste table here]

Although both Logistic Regression and SVM performed similarly in terms of AUC, Logistic Regression was selected for its faster training time and ease of interpretation.

## Key Insights (Based on Logistic Regression Coefficients)
[Paste chart with positive coef]

- March was the most impactful contact month. Customers contacted in MArch had the strongest positive influence on subscription likelihood, according to the model. This suggest that making campaigns in March are significantly more effective than in other months.


- Macroeconomic variables like cons.price.idx and euribor3m had positive influence.
Higher values of the consumer price index (cons.price.idx) and the 3-month Euribor rate (euribor3m) were associated with greater likelihood of subscription. This may reflect customer behavior during favorable economic conditions.

- Past campaign success was a strong predictor.
Customers who had a poutcome_success (successful outcome in a previous campaign) showed significantly higher odds of subscribing again, reinforcing the value of retargeting warm leads.

- Students, retirees, and university graduates were more likely to subscribe.
The features job_student, job_retired, and education_university.degree all appeared among the top positive coefficients, suggesting these demographic groups are more receptive to term deposit offers.


[Paste chart with negative coef]
- Some months were highly ineffective.
Contacting customers in May, November, and June had strong negative associations with conversions. These may be poor times for outreach due to seasonal behavior or distractions.

- Economic uncertainty reduced conversion odds.
A higher emp.var.rate (employment variation rate) was the strongest negative predictor, indicating that during unstable employment periods, customers were less likely to commit to term deposits.

- Communication channel matters.
Contacting customers via telephone (rather than cellular) was associated with significantly lower conversion likelihood — pointing toward the importance of using preferred or modern contact methods.

- Certain job categories were less responsive.
Customers working as entrepreneurs, in services, or in blue-collar occupations were less likely to subscribe, suggesting the need for tailored messaging or alternative products for these segments.

- Long gaps since last contact (pdays) hurt performance
A higher number of days since last contact correlated negatively with conversions, reinforcing the value of timely follow-ups in marketing.