# Fraud Detection ML Project
## Dataset-
This [link](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud?select=creditcard.csv) will take you to kaggle website from where you can download the .csv file.

## Introduction-
Traditional fraud detection techniques often rely on rule-based systems that require human experts to manually update the rules as new fraud patterns emerge. These methods can be time-consuming, expensive, and often fail to detect new and evolving fraud patterns.

Hence, we used various Machine Learning algorithms to identify evolving fraud patterns even in the presence of imbalanced data.

## Libraries used-
- numpy
- pandas
- sklearn
- matplotlib
- seaborn
- imblearn
- xgboost
- pylab

## Models used-
- Isolation Forest
- Local Outlier Factor
- Support Vector Machine
- Random Forest Classifier( with RandomUnderSampler and SMOTE as samplers )
- XGBClassifier

## 3 best Models with their Accuracy Rates-
- ## Isolation Forest- 
 Isolation Forest is a technique for identifying outliers in the dataset.The approach employs binary trees to detect anomalies, resulting in a linear time complexity and low memory usage that is well-suited for processing large datasets.
Our model shows an accuracy of 99.74% on test data with Isolation Forest.

- ## Random Forest Classifier-
Random Forest Classifier takes less training time as compared to other algorithms. It predicts output with high accuracy, even for the large dataset it runs efficiently. It can also maintain accuracy when a large proportion of data is missing. But, due to data imbalance, it was tending to ignore the minority class( Data with Fraud) which was the most important class in our case. Hence, we performed undersampling using RandomUnderSampler and oversampling using SMOTE.
Accuracy in both cases was 99.96 and 99.94 respectively.

- ## XGBClassifier-
 XGBoost stands for “Extreme Gradient Boosting”.XGB consists of a number of hyper-parameters that can be tuned — a primary advantage over gradient boosting machines. XGBoost has an in-built capability to handle missing values and it can be used for large datasets effectively.
 Our model showed an accuracy of 99.89 on test data with XGBClassifier.
 
 ## Conclusion-
 All the 3 above models explained above, show amazing results. We choose *Random Forest Classifier* as our final algorithm as it shows an overall better accuracy as compared to other 2. 
