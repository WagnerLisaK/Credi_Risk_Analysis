# Credit Risk Analysis

## Overview
This project was to analyze different models on predicting high risk credit applications.  Because credit risk is inherently unbalanced, there are many ways to handle this issue when predicting credit risk.  I analyzed the data using 6 different methodologies as shown below.

All numbers are a percentage (ex. 0.65 = 65%, ; 0.02 = 2%).

## Results
**1. Naive Random Oversampling**

     * Balanced Accuracy Score = 0.65 (overall accuracy)
     * Precision = 0.01  (accuracy of positive predictions)
     * Sensitivity/Recall = 0.69  (% of positive cases identified correctly)
     * F1 Score = 0.02  (% of correct positive predictions)

     ** Decent overall accuracy score; low accuracy of identifying high risk loans.**
     
![NaiveRandOverSamp.png](https://github.com/WagnerLisaK/Credit_Risk_Analysis/blob/main/Resources/NaiveRandOverSamp.png)

**2. SMOTE Oversampling**

     * Balanced Accuracy Score = 0.66
     * Precision = 0.01
     * Sensitivity/Recall = 0.63
     * F1 Score = 0.02

     ** Decent overall accuracy score; low accuracy of identifying high risk loans.**

![SMOTE.png](https://github.com/WagnerLisaK/Credit_Risk_Analysis/blob/main/Resources/SMOTE.png)

**3. ClusterCentroids Undersampling**

     * Balanced Accuracy Score = 0.54
     * Precision = 0.01
     * Sensitivity/Recall = 0.69
     * F1 Score = 0.01

     ** Mediocre overall accuracy score; low accuracy of identifying high risk loans.**

![ClusterCentroidsUnderSamp.png](https://github.com/WagnerLisaK/Credit_Risk_Analysis/blob/main/Resources/ClusterCentroidsUnderSamp.png)

**4. Combination Sampling**

     * Balanced Accuracy Score = 0.68
     * Precision = 0.01
     * Sensitivity/Recall = 0.78
     * F1 Score = 0.02

     ** Decent accuracy score; low accuracy of identifying high risk loans.**

![CombinationSamp.png](https://github.com/WagnerLisaK/Credit_Risk_Analysis/blob/main/Resources/CombinationSamp.png)

**5. Balanced Random Forest Classifier**

     * Balanced Accuracy Score = 0.79
     * Precision = 0.03
     * Sensitivity/Recall = 0.70
     * F1 Score = 0.06

     ** Good accuracy score; but still low accuracy of identifying high risk loans.**

![BalRanForClass.png](https://github.com/WagnerLisaK/Credit_Risk_Analysis/blob/main/Resources/BalRanForClass.png)

**6. Easy Ensemble AdaBoost Classifier**

     * Balanced Accuracy Score = 0.93
     * Precision = 0.09
     * Sensitivity/Recall = 0.92 
     * F1 Score = 0.16

     ** Great overall accuracy score; but still low accuracy of identifying high risk loans.**

![EasyEnsAdaBoostClass.png](https://github.com/WagnerLisaK/Credit_Risk_Analysis/blob/main/Resources/EasyEnsAdaBoostClass.png)


## Summary

Using over-, under-, and combination-sampling produced the least favorable accuracy results of predicting high credit risk.

The classifiers performed better, but neither had a high level of accuracy when predicting high credit risk.

The best at predicting high credit risk was the Easy Ensemble AdaBoost Classifier.  The overall accuracy score was 0.93, but the F1 score was still low at 0.16.

I would recommend one or more of the following moving forward:
1. Gathering more data to increase the size of the dataset;
2. Add more features that are more meaningful;
3. Specify the weight of each feature instead of letting the model do that;
4. Instead of predicting high risk applications, predict low risk applications instead, and re-run the models to see what impact that has on the predictions.

Submitted by Lisa K Wagner / 21 Oct 2021





