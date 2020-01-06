# Building a spam filter for SMS messages

The goal of this project is to build a spam filter that classifies SMS messages as spams or hams (i.e., non-spam messages).

The data set we will use to train and test our classifier is available in the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection).

The [dataset](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection) contains 5572 messages labelled as spam or non-spam (ham). 

We'll build the spam filter using the multinomial Naive Bayes Algorithm, and our goal is to reach an accuracy > 95%.

In this project we'll do the following:
- Split the dataset into a training set and a test set
- Create a vocabulary of the unique words of all the SMS messages in our dataset
- Convert the SMS messages into a word frequency matrix
- Calculate the constants and parameters of the Naive Bayes Algorithm
- Build the spam filter
- Measure the accuracy of the spam filter
