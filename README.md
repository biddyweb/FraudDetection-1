# FraudDetection using Logistic Regression
An analysis to predict whether a card transaction can be fraud or not using the Choice modeling. I did this as a part of helping an internal team at work with their Fraud modeling problem. The data used in this problem set are all dummy data sets and has nothing "production" about them.

About the Data: 500 Rows with Dummy card numbers along with a unique sequence ID for all the transactions against them. Transaction attributes/columns include the Zip Code, Merchant Category code, Amount involved in the transaction and whether the transaction was Fraud or not.

1) Data Visualization: Undersanding and verifying the underlying distribution of data. E.g. where Fraud or Not false, whether Amount has outliers and needs transformations. Types of variables - categorical or continuous

2) Data Scrubbing: Making sure all the data types are as expected (Float, int, string etc). In this case, creating dummy/indicator variables for the categorical variables.

3) Data exploration: Since it was choice modeling, Logistic regression was a straightforward choice but using statsmodels, I was running into errors of high collinearity and dimensionality. So used PCA to reduce dimensions before feeding it into the logistic regression fit.

4) Modeling: Once Logistic regression was established, then I use scikit learn to cross validate the regression results. For another step of validation, I also tried using KNN to see how the results yeild.

5) Interpretation: Interpreting the results and cross-validating the ccuracy of the predictions arising out of Logistic regression/KNN.
