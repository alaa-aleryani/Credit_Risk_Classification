# Credit Risk Classification Report

## Overview of the Analysis

For this analysis, we used some techniques such as `LogisticRegression` and `Resampling Method` to train and evaluate a model based on loan risk. We used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.


## Results 

* Machine Learning Model 1:
  * For the 1st Model, we used `LogisticRegression` with the `Original Data`.
  * We had an overall accuracy of 94%.
  * Precision for healthy loan labels is 100%, however, it is 87% for high risk loan labels.
  * Recall score for healthy loan labels is 100%, but 89% for high risk loan labels.


* Machine Learning Model 2:
  * For the 2nd Model, we also used `LogisticRegression`, but with a `Resampled Data`. 
  * Overall accuracy has increased from 94% to 99.6%.
  * Precision for healthy loan and risk loan labels remians the same, that is 100% and 87% respectively.
  * Recall score for healthy loan labels remains the same at 100%; however, for the high risk loan labels the recall has increased from 89% to 100%.

## Summary


