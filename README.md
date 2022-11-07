# Credit_Risk_Analysis

## Overview of the analysis

### This is an analysis using Machine Learning Algorithms to help identify credit risk.  The data that was used came from LendingClub in 2019.

### The purpose of this analysis was to understand how to use Supervised Machine Learning statistical algorithms to make predictions based on the patterns in data.  To complete this analysis we used 6 different models to evaluate which one would perform the best, if any, at predicting credit risk.  Those models were:
•	Naïve Random Oversampling
•	Smote Oversampling
•	Undersampling – Cluster Centroids
•	Smoteen(combination of over and under sampling)
•	Balanced Random Forest Classifier
•	Easy Ensemble AdaBoost Classifier

### Using these algorithms, the data was resampled and we calculated the accuracy score, confusion matrix(example shown below)  and classification report for each type.  

![Confusion_Matrix_ex](https://user-images.githubusercontent.com/106286533/192648912-47b59ab2-6181-42b3-a2b3-e884444215a0.png)

## Results

### To perform the analysis we used the “loan_status” column as our target data to determine whether the application was low or high risk.  If the application was current it was considered low-risk, and the remaining was high-risk.  The reduced dataset contained 68,817 applications distributed as follows:

![Y_Value_counts](https://user-images.githubusercontent.com/106286533/192648964-0c508ede-7d29-4d60-9fc5-22700432f7e6.png)

### The data was then split into Training and Testing sets at 75%/25% respectively.  

![Train_Test_Split](https://user-images.githubusercontent.com/106286533/192648981-289de3eb-76cc-45bf-b29b-9677b148f147.png)

### Naïve Random Oversampling – accuracy score was 64.4%

![Naive_Random_Oversampling](https://user-images.githubusercontent.com/106286533/192649014-180291f6-aca5-4a7c-bb7b-f0f4f4c67385.png)

### Smote Oversampling - accuracy score was 66.3%

![Smote](https://user-images.githubusercontent.com/106286533/192649037-55871660-8ac4-4153-8db8-e629504298db.png)

### Cluster Centroids Undersampling - accuracy score was 54.4%

![Undersampling](https://user-images.githubusercontent.com/106286533/192649067-5ddb6211-98e8-43b1-8fc6-99cf60a89435.png)

### Smoteen - accuracy score was 64.5%

![Smoteen](https://user-images.githubusercontent.com/106286533/192649097-df1054ee-9a69-4dba-a95a-640768be5e00.png)

### Balanced Random Forest Classifier - accuracy score was 78.9%

![Balanced_Random_Forest_Classifier](https://user-images.githubusercontent.com/106286533/192649121-4cf3192e-e251-47ce-995f-472dfecf922c.png)

### Easy Ensemble AdaBoost Classifier - accuracy score was 93.2%

![Easy_Ensemble_AdaBoost_Classifier](https://user-images.githubusercontent.com/106286533/192649154-2803f7f4-800d-40c1-8ee7-7b501eb16f67.png)

## Summary

### The Easy Ensemble AdaBoost model yielded the best results with a 93.2% accuracy score, 9% Precision and 92% recall on “High Risk” applications.  I would recommend this model to predict credit risk.  This was a clear choice as the accuracy scores on the other models were considerably lower.  The next highest score was 78.9% with the Random Forest. 

