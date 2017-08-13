# EmailClassification
##An implementation of Naive Bayes algorithm for email classification using Spark in Python.

The goal of this project is to achieve classification of spam and ham emails from the Enron Email Dataset.

Classification is a supervised learning algorithm. I set out to implement this project for having an experience as to how email classification is implemented on various email applications. I have implemented Naive Bayes Classification for classification. Efficiency of the project was calculated using metrics: Accuracy, Precision and Recall and F-Measure. 

* Motivation: The main motivation for the project is to work on raw data as it was obtained. I took text of emails as it is and performed analysis on it using various libraries and algorithms. This way, data did not need to be processed before using it. It was definitely interesting to understand the problem at hand since we used textual information, processing it in the algorithm was a challenge.

* Dataset: I used processed data from Enron email dataset. It contains already separated emails with labels 'spam' and 'ham'. For this project I have used small subset of data available. I have total of 3024 ham and 1500 spam emails in training set and we evaluate 648 ham and 256 spam mails from test set.
You can find dataset [here.](http://www.cs.cmu.edu/~enron/)

* Frameworks: 
  * Apache Spark - PySpark framework was used for this project.  
  * Spark version used : 1.0.6
  * Python version: 2.6


* Performance Evaluation: The performance of the system is measured in terms of Accuracy, Precision and Recall. The details of these metrics are given below:
  * Accuracy = Accuracy (A) is the percentage of all emails that are correctly categorized. Total number of emails correctly classified /  Total number of emails
  * Precision = It is the number of relevant documents identified.The precision is intuitively the ability of the classifier not to label as positive a sample that is negative. Total number of emails correctly classified as either ham or spam / Total number of spam/ham emails
  * Recall = It is the percentage of all spam emails that are correctly classified as spam. The recall is intuitively the ability of the classifier to find all the positive samples.  It is calculated as: Number of spam/ham correctly classified / Total number of messages.
* F-measure = F measure is a combined measure that assesses the precision and recall trade off and is basically a weighted harmonic mean of precision (P) and recall (R).

* Results:
  * Accuracy = 0.830752 
  * Precision = 0.830752
  * Recall = 1.0 
  * F-measure = 0.907552
