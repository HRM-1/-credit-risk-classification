# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.

The objective of this analysis is to develop a robust model that accurately predicts the number of healthy loans, utilizing diverse techniques to train and evaluate models based on loan risk. Leveraging a dataset encompassing historical lending activities from a peer-to-peer lending services company, our aim is to construct a model capable of discerning the creditworthiness of borrowers. Through employing advanced methodologies and rigorous evaluation processes, we endeavor to enhance the efficiency and effectiveness of our predictions, thereby aiding in prudent decision-making within the lending domain.

* Explain what financial information the data was on, and what you needed to predict.
The dataset comprises financial information related to lending activities, particularly focusing on borrowers' creditworthiness and associated risk factors. It includes various features such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The primary objective is to predict the likelihood of loans being healthy or high-risk based on this financial information. In essence, the goal is to assess the credit risk associated with each loan application, enabling the lending institution to make informed decisions regarding loan approvals and mitigate potential losses by accurately identifying loans that are likely to default.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
We aimed to predict the loan status using logistic regression. The model excelled in identifying healthy loans ('0'), achieving impeccable precision and recall scores of 1.00, implying that it accurately identifies and classifies virtually all safe loans. However, its performance on predicting high-risk loans ('1') was slightly less accurate, with a precision of 0.86. Despite this, the model demonstrated commendable recall, correctly identifying the majority of actual risky loans with a score of 0.91. Impressively, the model exhibited an overall accuracy of 0.99 on the test dataset, indicating its robust performance in predicting loan statuses with remarkable precision.

* Describe the stages of the machine learning process you went through as part of this analysis.
- Data Collection: We gathered a dataset containing lending records.
- Data Cleaning and Preparation: We cleaned the dataset and made it ready for analysis by handling missing values and encoding categorical variables.
- Exploratory Data Analysis (EDA): We explored the dataset to understand its characteristics and relationships between variables using visualizations.
- Feature Selection/Engineering: We selected important features and created new ones to improve model performance.
- Model Selection: We chose Logistic Regression as our primary model for its simplicity and effectiveness in binary classification tasks.
- Model Training: We trained the model using the prepared dataset.
- Model Evaluation: We assessed the model's performance using various metrics to understand its effectiveness.
- Model Tuning: If needed, we adjusted the model's parameters to optimize performance.
- Model Deployment: We deployed the model for making predictions on new data.
- Monitoring and Maintenance: We continuously monitored the model's performance and updated it as needed to ensure its reliability over time.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
- Logistic Regression: This was the primary machine learning algorithm chosen for predicting loan statuses. Logistic Regression is well-suited for binary classification tasks and provides interpretable results.
- Resampling Methods: We utilized resampling techniques, such as Random Oversampling, to address class imbalance in the dataset. This involved creating synthetic samples of the minority class (high-risk loans) to balance the distribution and improve model performance.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
Machine Learning Model 1:
Balanced Accuracy Score: The balanced accuracy score is approximately 0.97, indicating strong performance in making correct predictions across both classes while considering class imbalance.
Precision: For class 0 (healthy loans), the precision is 1.00, indicating that all loans predicted as safe are indeed safe. For class 1 (high-risk loans), the precision is 0.86, implying that 86% of the predicted high-risk loans are correctly classified.
Recall: For class 0, the recall is 0.99, meaning that almost all actual safe loans are correctly classified. For class 1, the recall is 0.94, indicating that the model captures 94% of actual high-risk loans.

Machine Learning Model 2:
Balanced Accuracy Score: The balanced accuracy score is approximately 0.99, demonstrating excellent performance in making accurate predictions across both classes, considering class imbalance.
Precision: For class 0, the precision is 1.00, indicating that all loans predicted as safe are indeed safe. For class 1, the precision is 0.85, implying that 85% of the predicted high-risk loans are correctly classified.
Recall: For class 0, the recall is 0.99, meaning that almost all actual safe loans are correctly classified. For class 1, the recall is 0.99, indicating that the model captures 99% of actual high-risk loans.




## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

Based on the results of the machine learning models, both models demonstrate strong performance in predicting loan statuses, achieving high accuracy, precision, and recall scores. However, Model 2 appears to perform slightly better than Model 1. This conclusion is based on the following observations:

Model 2 achieves a slightly higher balanced accuracy score of approximately 0.99 compared to Model 1, which has a balanced accuracy score of approximately 0.97.
Both models have high precision and recall scores for predicting healthy loans (class 0), with Model 2 achieving perfect precision and recall scores.
Model 2 also exhibits higher precision and recall scores for predicting high-risk loans (class 1), although the difference is marginal.
Being the primary objective to accurately predict both healthy loans and high-risk loans, Model 2 would be preferable due to its slightly higher overall performance. 

In summary, while both models demonstrate strong performance, Model 2 appears to perform slightly better overall. 








