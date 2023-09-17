# Credit-risk-classification


Background
In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

- Split the Data into Training and Testing Sets

- Create a Logistic Regression Model with the Original Data

- Write a Credit Risk Analysis Report:

Upon initial review, more borrowers repaid (75036) than defaulted (2500). This imbalance could affect model performance on the smaller dataset. To address this, we split the data, set up the model parameters, and conducted training and prediction.

Additionally, we used RandomOverSampler to balance dataset proportions for improved default prediction.

Results:

Model 1:

- Balanced Accuracy: 0.952
- Precision (Healthy Loans/High-risk Loans): 1.00/0.85
- Recall (Healthy Loans/High-risk Loans): 0.99/0.91


Model 2 (resampled):

- Balanced Accuracy: 0.994
- Precision (Healthy Loans/High-risk Loans): 1.00/0.84
- Recall (Healthy Loans/High-risk Loans): 0.99/0.99

Summary:

Both models performed well with scores mostly above 80%. Model 2 which utilized the resampled dataset, outperformed Model 1. Achieving a balanced accuracy of 0.99 compared to 0.95. Notably, it significantly reduced false negatives for high-risk loans (from 56/563 to 4/615). Given the priority of avoiding default, we recommend using logistic regression with resampled data for more accurate approval decisions.




Homework completed with the help of class activities files and google/chatgpt.
