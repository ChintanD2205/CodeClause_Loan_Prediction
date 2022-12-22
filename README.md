# CodeClause_Loan_Prediction
For the loan prediction task I used mainly 3 libraries namely numpy, pandas and matplotlib.

I stored 2 datasets, 1 for training and other for testing.
First, I checked whether there are any null values in the data or not and checked for any outliers. 
For outliers, I normalized the data using log function and filled the null values using mode and mean functions while keeping inplace=True.
Once all values were not null, the complete dataset was divided into two parts i.e dependent and independent.

After separation, I used train_test_split to further categorically split the data into training and testing sides.
Further, I used label encoding to convert the text data into numerical values to help with prediction.

After that I compared 2 algorithms i.e. Decision Tree Classifier and Naive Bayes Classification with the help of metrics.accuracy_score() and it revealed that the Naive Bayes algorithm was much more efficient.
So for the final prediction on the test dataset we use the Naive Bayes Classifier and predict whether a particular user would receive a loan or not.
