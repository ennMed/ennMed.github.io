# Fraud detection (compet)

## 1 Introduction
In this markedown, we compared different machine learning models on a large-scale dataset. The data comes from actual company "X"  e-commerce transactions and contains a wide range of features from device type to product characteristics. The goal here is to improve the effectiveness of fraudulent transaction alerts by predicting the probability that an online transaction is fraudulent, i.e., to predict the value of the binary target ***isFraud***

## 2 Data analysis

To predict our target variable, isFraud, we have two tables. Indeed, the data are divided into two files: identity and transaction, which are linked by a key: TransactionID. Not all transactions have corresponding identity information. The transaction table has 394 characteristics and 590540 observations while identity has 41 characteristics and 144233 observations. The two tables have both category and category-like variables. The two tables have both category and continuous variables.
The transaction table gathers the different information attached to a transaction such as the amount.


The variables of the identity table are, as for them, information on the identity, the connection to the network and the digital signature associated with the transactions. Nous n'avons pas accès au d'etail We do not have access to the details of the field names, they are hidden for privacy reasons.
privacy. We first started our exploration of the data by noting that the proposed dataset was not a complete one.


Data set was imbalanced. As you can see from the pie chart Figure 1, the non-fraudulent transactions far outweigh the fraudulent transactions. In
Indeed 96% of the transactions in the dataset are not fraudulent. If we train a binary classification model without solving this problem, the model will be completely biased.


Then we were interested in the missing values. We noticed that our data had a lot of missing values. As Figure 2 shows, some variables have more than 99% of missing values.





