# Credit_Risk_Analysis
## Overview
For this analysis, I created supervised machine learning models to assist in predicting credit risk. I tested six different methods including: Naive Random Oversampling, SMOTE Oversampling, Cluster Centroid Undersampling, SMOTEENN Sampling, Balanced Random Forest Classifying, and Easy Ensemble Classifying. I then evaluated my results of these models to make a recommendation on whether a certain model should be used to predict credit risk. 


## Results

### Naive Random Oversampling
- Accuracy Score: 65.5
- Precision High Risk: 1%
- Precision Low Risk: 100%
- Recall High Risk: 70%
- Recall Low Risk: 61%
![Naive_Random](https://github.com/MeredithTracy/Credit_Risk_Analysis/blob/main/Images/Naive_Random.png)

### SMOTE Oversampling
- Accuracy Score: 66.2%
- Precision High Risk: 1%
- Precision Low Risk: 100%
- Recall High Risk: 63%
- Recall Low Risk: 69%
![SMOTE](https://github.com/MeredithTracy/Credit_Risk_Analysis/blob/main/Images/SMOTE.png)

### Cluster Centroid Undersampling
- Accuracy Score: 54.4%
- Precision High Risk: 1%
- Precision Low Risk: 100%
- Recall High Risk: 69%
- Recall Low Risk: 40%
![ClusterCentroids](https://github.com/MeredithTracy/Credit_Risk_Analysis/blob/main/Images/ClusterCentroids.png)

### SMOTEENN Sampling
- Accuracy Score: 67.1%
- Precision High Risk: 1%
- Precision Low Risk: 100%
- Recall High Risk: 76%
- Recall Low Risk: 58%
![SMOTEENN](https://github.com/MeredithTracy/Credit_Risk_Analysis/blob/main/Images/EE_Class.png)

### Balanced Random Forest Classifying
- Accuracy Score: 68.3%
- Precision High Risk: 88%
- Precision Low Risk: 100%
- Recall High Risk: 37%
- Recall Low Risk: 100%
![Bal_Ran_Forest_Class](https://github.com/MeredithTracy/Credit_Risk_Analysis/blob/main/Images/EE_Class.png)

### Easy Ensemble Classifying 
- Accuracy Score: 93.2%
- Precision High Risk: 9%
- Precision Low Risk: 100%
- Recall High Risk: 92%
- Recall Low Risk: 94%
![EE_Class](https://github.com/MeredithTracy/Credit_Risk_Analysis/blob/main/Images/EE_Class.png)

## Summary 

Based on our results, we can see that the Easy Ensemble Classifier model has the highest recall for high risk loans at 92% followed by the SMOTEENN model at 76%. This means that it is a sensitive model so its detecting a majority of high risk loans that pass through it.  

The Easy Ensemble Classifier model has the highest accuracy score at 93.2% followed by the Balanced Random Forest Classifer model at 68.3%. 

Even though we had success with creating sensitive models, the only model that had good precision in catching high risk loans was the Balanced Random Forest Classifier model at 88%. 

The models who did the best in sensitivity had low precision and the penalty for falsely labeling a low risk loan as high risk may not be worth it to a bank overall. If a bank plans on using this as a first step in looking at credit risk, the sensitive models would be great because we know we are catching the high risk loans that pass through. I would recommend the Easy Ensemble Model. 
But if they are using this model as their only prediction for credit risk, I would not make a recommendation because the only one who scored highly on precision for high risk loans, doesn't have a good score sensitivity for high risk loans (37%) and its only has a 68.3% for accuracy. 
