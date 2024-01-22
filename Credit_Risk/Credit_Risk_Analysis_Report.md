# Credit Risk Classification Report

## Overview of the Analysis

For this analysis, we used some techniques to train and evaluate a model based on loan risk. We used `LogisticRegression` because the prediction is categorical and `Resampling Method` to handle the imbalanced data, where we had more 0's (healthy loan applicants) than 1's (high risk loan applicants). The purpose was to have a trusted model that gives us a high recall for the healthy and risky loan applicants. Thus, we used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.


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

Although the first model gave us 94% accuracy, it's just that the recall for the high risk applicants that is 89% compared to the recall of 100% for the low risk applicants. That was something not practical and not what we wanted. I wanted the recall for High Risk applicants to be as high as well. Thus, I used the `RandomOverSampler` module from the imbalanced library to `resample` the data then create the second model.
Now, with the over sampled data, overall accuracy has increased from 94% to 99.6% almost 100%. And the recall for risky loans has also increased from 89% to 100%. Thus, now the model is something that can be trusted specially in the case of risky loan applicants. Overall, the second model with the `Resampled Data` performed better because it gave us high overall accuracy as well as high recall for both risky loan and healthy loan applicants.
