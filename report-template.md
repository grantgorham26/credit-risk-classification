# Module 12 Report 

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* The purpose of this challenge was to take some data about a person who is applying for a loan and train a machine learning model on this data to determine whether a person is likely to get a loan or not. 

* Explain what financial information the data was on, and what you needed to predict.
The financial data included the size of the loan, the specific interest rate fo the loan, income of the borrower, a debt to income ratio, the number of accounts of the borrower, the number of deragatory marks on a borrowers account, the borrowers total debt, and whether the borrowe was approved for the loan. Using this data we are trying to determine whether someone is likley to be approved or not be approved for a loan. 

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
The variable we are trying to predict is whether a person will qualify for a loan. 

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).
logistric regression is a training alogrithim that uses one vs the rest scheme. the logistic regression class implements regularized logistic regression using the 'liblinear' library, 'newton-cg', 'sag', 'saga' and 'lbfgs' solvers. 
## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
    Accuracy:.99. This means that the model is correct 99% of the time but his largely has to due with the imbalanced dataset we were using. 

    Healthy_loans(0)
    -precison:1.0.This means that when precicting a healthy loan the model will predict it with 100 percent accuracy 
    -recall:1.0. This essentially means that there are no false negatives predicted and the model perfectly identifies all the correct instances of the postive class.
    These scores are very skewed again because there are so many more cases of healthy loans. 

    unhealthy_loans(1)
    -precison:.87. 
    -recall:.89.


## Summary
When looking at how the model performs just by looking at the scores it seems like it would be very effective but when you start looking at the data that was used to train the model that changes. Since the data set is so skewed when separating healthy and unhealthy loans I can't make a confident recoomendation on whather this model should be used. A good next step would be to find another dataset that is more balanced and then train the model with that balanced data set. After this I could make a better reccomendation on the model. 
