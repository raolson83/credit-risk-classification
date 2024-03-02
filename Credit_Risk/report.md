# Module 12 Report Template

## Overview of the Analysis

In this analysis, we will analyze lending data that include indepedent financial variables that will predict the dependent binary variable of "healthy loan" or "high risk loan". This will be done first by running a logistic regression on the raw data after splitting into testing and training sets. However, it is known that the data is impbalanced, with many more instances of healthy loans than high risk loans. For this reasons, a second logistic regression will be performed untilizing an oversampling approach to balance the data. Results of the two analyses will be compared using a balanced accuracy measure. Analysis will be accompanied by confusion matrices and classification reports. 


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1 - Raw data: 
  * Balanced accuracy: .970
  * Precision: 0.92
  * Recall: 0.97


* Machine Learning Model 2 - Oversampled data:
  * Balanced accuracy: 0.993
  * Precision: 0.92
  * Recall: 0.99

## Summary

Model 1
With an F1 score of 1.0, prediction of healthy loans are predicted very well. The F1 score for high-risk loans is lower at 0.88, so the prediction is not as good, though this score may still be considered a successful result. This is likely do the imbalanced nature of the dataset, which has many more instances of healthy loans than high risk loans, and therefore much more data to train on for the former. The algorithm was more likely to misclassify a high risk loan as healthy than to misclassify a healthy loan as high-risk. 

Model 2
With an F1 score of 1.0, prediction of healthy loans are predicted very well. The F1 score for high-risk loans is lower at 0.91, so the prediction is not as good, though this score may still be considered a successful result. The oversampled dataset performs better for both high-risk loans and health loans than the regular datasets. However, the algorithm was still more likely to misclassify a high risk loan as healthy than to misclassify a healthy loan as high-risk. 

Conclusion: Overall, the oversampled logistic regression is stronger.  
