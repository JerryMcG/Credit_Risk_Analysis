# Credit_Risk_Analysis

## Overview
The purpose of this analysis is to compare different models and determine which is most useful for using in loan/credit prediction analysis.

## Results

* RandomOverSampler
1. Balanced Accuracy Score: 0.53
2. Precision: 0.99
3. Recall: 0.37

<img src = 'images/RandomOverAccuracy.jpg'/>
<img src = 'images/RandomOverClass.jpg'/>

* SMOTE
1. Balanced Accuracy Score: 0.53
2. Precision: 0.99
3. Recall: 0.41

<img src = 'images/SMOTEAccuracy.jpg'/>
<img src = 'images/SMOTEClass.jpg'/>

* ClusterCentroids
1. Balanced Accuracy Score: 0.54
2. Precision: 0.99
3. Recall: 0.36

<img src = 'images/CCAccuracy.jpg'/>
<img src = 'images/CCClass.jpg'/>

* SMOTEEN
1. Balanced Accuracy Score: 0.52
2. Precision: 0.99
3. Recall: 0.40

<img src = 'images/SMOTEENAcc.jpg'/>
<img src = 'images/SMOTEENclass.jpg'/>

* BalancedRandomForestClassifier
1. Balanced Accuracy Score: 0.61
2. Precision: 0.99
3. Recall: 0.59

<img src = 'images/BRF_Accuracy.jpg'/>
<img src = 'images/BRF_Classification.jpg'/>

* EasyEnsembleClassifier
1. Balanced Accuracy Score: 0.61
2. Precision: 0.99
3. Recall: 0.59

<img src = 'images/EnsembleAccuracy.jpg'/>
<img src = 'images/EnsembleClassification.jpg'/>

## Summary:

In general the random undersampling provided by BalancedRandomForestClassifier and EasyEnsembleClassifier worked a better in terms of a higher accuracy score and higher recall when compared with the different sampling models. The precision of all is quite high, which is a good thing due to the type of predictions we are making. We want to ensure that we are precise when determining who is a good candidate for a loan/credit. 

As a result, I would recommend either of the Ensemble models but with a word of caution since the Balanced Accuracy Score is not particularly high with a result of 0.61 for both models. 