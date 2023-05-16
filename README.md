# credit-risk-classification
Module 20 Challenge - DUE May 17, 2023

    ![]()

Business losses are common and each business needs to have tools to help predict what the customers need and want yet protect their own resources in the process. Today's assignment utlizes a dataset about loans which are healthy or high risk.  Our goal is to find a model to make these predictions.

There are two parts to this submission. The first part, credit_risk_classification satisfies the assignment code requirement and credit_risk_classification_extra satisfies additional curiosities. The Credit Risk Classification Analysis report takes both findings into account as does this README file.

The credit_risk_classification jupyter notebook begins with importing the modules and the csv file directly to a pandas DataFrame. Histograms plotted to view the data commonalities or not. We created the dependant variable y from the loan status, and the independant variable X from the features: loan size, interest rate, borrower income, debt to income, number of accounts, negative remarks, and total debt. We verified the counts of both variables. This dataset is then split into training and testing datasets. We create a Logistic Regression Model with the original data and then create one with data run through the RandomOverSample model specifically targeting the lesser class group of data. We created a confusion matrix, calculated the accuracy score (and balanced accuracy score) and the classification report for the model. In each case a question was answered.

The credit_risk_classification_extra jupyter notebook is an extension of the original assignment utilizing the dask DataFrame to import the csv file and by creating additional models because we were curious about how different models might affect our response to the assignment questions. We did find this to be useful and it is noted in the report.

The Credit Risk Classification Analysis report contains detail about how we organized our research and the final analysis.


## references

## machine learning from freeCodeCamp.org
- https://www.youtube.com/watch?v=i_LwzRVP7bg
code ideas and some code will be the same as this was assignment is expected to be my go to for example code when needed

## documentation on supervised learning
-https://scikit-learn.org/stable/tutorial/statistical_inference/supervised_learning.html

## classification report details
- https://medium.com/@kohlishivam5522/understanding-a-classification-report-for-your-machine-learning-model-88815e2ce397#:~:text=The%20classification%20report%20visualizer%20displays,was%20positive%20and%20predicted%20positive
   ## understanding of report details
 PRECISION - What percent of your predictions were correct?
  accuracy of positive predictions
 RECALL - What percent of the positive cases did you catch?
  fraction of positives that were correctly identified.
 F1-SCORE - What percent of positive predictions were correct?
  a weighted harmonic mean of precision and recall

## BCS Learning Assistant, Celine Wang
- pointing out the obvious, yet again :) and making the time to explain why

## BootCamp Instructor, Will and Learning Assitants, Michelle, Salman, and Yasmine
- without whose help and guidance, I wouldn't be 'hungry for more'

## high risk loans
- https://www.dccu.us/blog/main-advantages-and-disadvantages-of-high-risk-loans/#:~:text=In%20short%2C%20a%20high%2Drisk,them%20called%20bad%20credit%20loans

