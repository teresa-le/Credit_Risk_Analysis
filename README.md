# Credit Risk Analysis

## Purpose
The purpose of this analysis was to develop multiple supervised machine learning models to predict credit risk and determine which one(s) performed the best. The models were developed using different techniques to resolve the class imbalance issues; the number of low risk loans greatly outnumbered the number of high risk loans in the dataset. 

## Results

### Random Oversampling
* <b>Balanced accuracy score:</b>0.657
* <b>Precision:</b> 0.01 
* <b>Recall:</b> 0.71 

### SMOTE Oversampling
* <b>Balanced accuracy score:</b> 0.662
* <b>Precision:</b> 0.01 
* <b>Recall:</b> 0.63

### Cluster Centroids Undersampling 
* <b>Balanced accuracy score:</b> 0.544
* <b>Precision:</b> 0.01 
* <b>Recall:</b> 0.69

### SMOTEEENN Combination Sampling 
* <b>Balanced accuracy score:</b> 0.645
* <b>Precision:</b> 0.01 
* <b>Recall:</b> 0.72 

### Balanced Random Forest Classifier 
* <b>Balanced accuracy score:</b> 0.789
* <b>Precision:</b> 0.03 
* <b>Recall:</b> 0.70 

### Easy Ensemble AdaBoost Classifier 
* <b>Balanced accuracy score:</b> 0.932
* <b>Precision:</b> 0.09 
* <b>Recall:</b> 0.92 

Based on the balanced accuracy scores, the AdaBoost algorithm performed the best in terms of accurately predicting the classes, and the cluster-based undersampling technique performed the worst. 

All the models have fairly low precision scores when it comes to high risk applications, which indicates there were many false positives.  

The model that used the AdaBoost algorithm has the the best recall score (0.92) when it comes to high risk applications. On the other hand, the model produced using the SMOTE oversampling technique has the worst recall score (0.63). The recall score of the AdaBoost model is very high indicating that there weren't many false negatives. 

## Summary 
Out of the 6 machine learning models, the model that used the AdaBoost algorithm has the best score when it comes to balanced accuracy, precision and recall. 

Although it has a fairly low precision score, it has a high recall score. In this situation, recall is more important than precision because the lending company doesn't want to lose money by giving loans to people who are high risk and more likely to default on their loans. On the other hand, the company may miss out on potential opportunities by rejecting good loans. 

Therefore, I recommend that revisions be made to see if additional changes can be made to increase the precision score of the model without significantly decreasing accuracy. 