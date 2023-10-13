# Chrun Prediction
This work makes comparison of 4 models: Logistic Regression (LR), Random Forest (RF), K-Nearest Neighbors (KNN) and XGBoost. However, there is a problem of imbalance of data, so we will implement SMOTE (Synthetic Minority Over-sampling Technique), Over sampling and under sampling to all models. The objective of this test is to find the best model technique by considering with f1 score (Presision and recall), and Area Under the ROC Curve (AUC).

Dataset:
![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/68c2a6d55df8bdb8176fa160350be111ddb46f3f/03_Customer%20and%20Churn%20Scoring/Figures/Figure_001.png)

Running results:
![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/68c2a6d55df8bdb8176fa160350be111ddb46f3f/03_Customer%20and%20Churn%20Scoring/Figures/Figure_002.png)
To summarize the results above, the running results are gathered in the table below for analysis.
![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/68c2a6d55df8bdb8176fa160350be111ddb46f3f/03_Customer%20and%20Churn%20Scoring/Figures/Figure_003.png)
Referring to the table above, it shows that XGboost (without balancing sample technique) is the best technique, because f1-score (both support 0 and 1) of this model has the highest score and even if its AUC for train is not the highest score, but AUC for test is the highest one. These indicates that XGboost model has the best ability to handle unknown data among theses crossing techniques.
