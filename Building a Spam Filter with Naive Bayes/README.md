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

The multinomial Naive Bayes algorithm we'll implement is the following:

\begin{equation}
P(Spam | w_1,w_2, ..., w_n) \propto P(Spam) \cdot \prod_{i=1}^{n}P(w_i|Spam)
\end{equation}
where $P(Spam | w_1,w_2, ..., w_n)$ is the probability a message is a spam, given its words, and $P(w_i|Spam)$ is the probability a word occurs in the message, given it is a spam. 

The same reasoning is then applied to estimate the probability a message is not a spam.

\begin{equation}
P(Ham | w_1,w_2, ..., w_n) \propto P(Ham) \cdot \prod_{i=1}^{n}P(w_i|Ham)
\end{equation}
