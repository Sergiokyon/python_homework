# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

The logistic regression model worked very well predicting both `0` (healthy loan) and `1` (high-risk loan) labels, but We have to take into consideration the fact that the data is imbalanced, and that might explain why the precision and recall metrics are almost perfect for the healthy loan since more than 95% percent of the data relies on this label even though high-risk loan also had high accuracy, I think the data needs to be more balanced in order to determine a better precision level on the model.


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

The logistic regression model fitted with the oversampled data seems to predict the `0` (healthy loan) and `1` (high-risk loan) labels very well. Since the data was balanced with this oversampled method, It is clear that this represents a more accurate model precision, with an f1 score of 1.00 for predicting a healthy loan and an f1 score of 0.91 for predicting high risk. In this specific case, recall is a more relevant metric than precision because the company wants to effectively identify high-risk loans to minimize bad loans since it could lead to significant financial losses. Inversely, in case the company wants to focus more on customer satisfaction, precision is crucial since it reduces the chances of a healthy loan being flagged as high-risk, which could lead to customer dissatisfaction and reputation damage. It all depends on the company's main objectives.


## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.


Both Machine learning models are helpful for this analysis (Identifying high-risk and healthy loans). Model 2 seems more accurate since the data is balanced, unlike Model 1. Also, if the company is looking to avoid financial risks such as default on loans, it should focus more on a model with a high recall score to effectively flag high-risk loans. If the only two available options were these two models, Model 2 would be the go-to since the data is balanced and has high accuracy, making it useful for the analysis in scope.