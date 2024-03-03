## Overview of the Analysis

This analysis was prepared using supervised machine learning algorithms to examine the creditworthiness of customers and their relative riskiness as a potential loan borrower. The model is trained by past bank data, to identify the factors that lead to default. Among the criteria considered as predictive features for potential loan health are the following:

<ul>
    <li>The size of the loan</li>
    <li>The interest rate of the loan</li>
    <li>The borrower's income</li>
    <li>The borrower's debt to income ratio</li>
    <li>The number of accounts for each borrower</li>
    <li>The number of derogatory marks on any of the borrower's accounts</li>
    <li>The borrower's total debt</li>
</ul>

From this information, the model is predicts whether or not a potential loan would be a likely default using the following methodology: 

The data were pulled from 77,536 customer records, from which 3.2% were in default and 96.8% were in good standing. 

These data were then split into training (75%) and testing (25%) sets, maintaining the ratio of good standing and default loans from the orignial dataset. The training set was then used to fit the logistical regression model. Once trained, predictions were created by the model from the remaining test set and the accuracy (precentage of correct predictions), precision (the quality of a positive prediction made by the model), and recall(frequency of correctly identifying a positive instance) were measured in order to gauge the effectiveness of the model.  

Due to the inbalanced nature of the training and testing data, a random over sampler was then used to increasing the number of the minority class (defaults). The preceeding steps were then repeated with this resampled dataset to examine the differences in training methods and each model's effectiveness.

## Results

<ul> 
    <li>Machine Learning Model 1: Original Linear Regression</li>
    <li><ul>
        <li>Accuracy: .994</li>
        <li>Prescision: 
        <ul>
            <li>non-default: 1.0</li>
            <li>default:.87</li>
            <li>weighted average: .99</li>
        </ul>
        </li>
        </ul>
    </li>
</ul>



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
