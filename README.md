# Credit_Risk_Analysis
Fast Leaning, a peer to peer lending firm has engaged Garner INC to develop a supervised machine learning model.  The objective of this project is to assess credit risk for potential load defaults. 

##Resources - 
- Software - Python 3.7.13, GitBast, GitHub, Conda 4.8.4, Jupyter Notebook 6.4.12
- libraries - scikit-learn and imbalanced-learn
- algorithims - 
    - oversampling - RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN
    - undersampling
    - combo oversampling and undersampling
    - models - BalancedRandomForestClassifier and EasyEnsembleClassifier, Linear Regression
- Data - LoanStats_2019Q1.csv

## Results & Analysis
Data was read in from the file "C:\Users\karla\Documents\GitHub\Credit_Risk_Analysis\LoanStats_2019Q1.csv" and cleaned for modeling and testing.  Analysis was conducted utilizing supervised machine learning over a range of algorithms including oversampling, undersampling, and combination methods.  Outputs were as follows.

### RandomOverSampleing model
https://github.com/KJAnalytics/Credit_Risk_Analysis/blob/main/Images/Naive_Random_oversampling_accuracy.jpg
https://github.com/KJAnalytics/Credit_Risk_Analysis/blob/main/Images/Naive_Confusion_Matrix_imbalanced_classification_report.jpg

Balanced Accuracy Score: 63%
Precision Scorea:
High Risk: 1%
Low Risk: 100%
Recall Score:
High Risk: 57%
Low Risk: 68%


### SMOTE model
https://github.com/KJAnalytics/Credit_Risk_Analysis/blob/main/Images/Smote_Accuracy_confusion_classification.jpg

Balanced Accuracy Score: 63%
Precision Scores:
High Risk: 1%
Low Risk: 100%
Recall Score:
High Risk: 62%
Low Risk: 63%

###ClusterCentroids model
https://github.com/KJAnalytics/Credit_Risk_Analysis/blob/main/Images/Undersampling_outputs.jpg

Balanced Accuracy Score: 53%
Precision Scores: 
High Risk: 1%
Low Risk: 100%
Recall Score:
High Risk: 61%
Low Risk: 45%

###  SMOTEENN
https://github.com/KJAnalytics/Credit_Risk_Analysis/blob/main/Images/Combo_over_under_outputs.jpg

Balanced Accuracy Score: 62%
Precision Score:
High Risk: 1%
Low Risk: 100%
Recall Score:
High Risk: 70%
Low Risk: 54%

### Balanced Random Forest Classifier
https://github.com/KJAnalytics/Credit_Risk_Analysis/blob/main/Images/BRFC_Model_confusion_matrix_classification_report.jpg

Balanced Accuracy Score: 79%
Precision Score:
High Risk: 4%
Low Risk: 100%
Recall Score:
High Risk: 67%
Low Risk: 91%

### Easy Ensemble AdaBoost Classifier
https://github.com/KJAnalytics/Credit_Risk_Analysis/blob/main/Images/Confusion_Matrix_classification_report_ADABoost.jpg

Balanced Accuracy Score: 93%
Precision Score:
High Risk: 7%
Low Risk: 100%
Recall Score:
High Risk: 91%
Low Risk: 94%
## Summary and Takeaways 
In each of the models performed, the credit risk high has weak presitions.  We see improvements in the use of the Ensemble models over other models evaluated.  In these Ensemble models, we see high recall results for the higher risk loan category, but that is a trade off as there is still a risk of the lower risk credit statuses resulting in false positives.

From the bank perspective the Easy Ensemble Classifier model would be recommended from the models tested.  With a 93% accuracy score it is a top performer for detecting the high rick category loans.  

I personally would prefer that none of these models be used, as the potential is present that many good lendees who would pay their loans on time would be turned away based on these models.  

Both of thes situations would need to be weighed by the Fast Lending team as both situations have issues on their financial bottom line.

