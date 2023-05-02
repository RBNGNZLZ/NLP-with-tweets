# Natural Language Processing with Disaster Tweets

## Mission 
The task is to develop a machine learning model that can classify tweets about real
disasters or not. The tweets in the dataset have been hand-classified, and the goal is
to create a model that can accurately classify new, unseen tweets. The challenge is
that some tweets may contain words that are commonly associated with disasters,
but are not actually about real disasters. For example, a tweet containing the word
"ABLAZE" may be metaphorical and not refer to a real fire.

## Machine Learning Task
This is a binary classification task. Given the text, keyword, and location of a tweet, the model
needs to predict whether the tweet is about a real disaster or not.
ML Method
To determine the best machine learning method to use for this project, we will be experimenting
with the following. Convolutional Neural Networks (CNNs), Random Forest, Logistic
Regression, and Naive Bayes.

## Evaluation Method
We will be using the F1 score as the evaluation metric, which is the harmonic mean of precision
and recall. The F1 score balances both precision and recall and is a good metric for
imbalanced datasets. The higher the F1 score, the better the model's performance.
Data
The dataset consists of three CSV files: train.csv, test.csv, and sample_submission.csv. The
training set contains 7,613 tweets and the test set contains 3,263 tweets. Each tweet is
represented by its text, a keyword (which may be blank), and the location from which it was
written (which may also be blank). The training set also includes a target column, which indicates
whether the tweet is about a real disaster or not.

### Data Columns
- id - a unique identifier for each tweet
- text - the text of the tweet
- location - the location the tweet was sent from (may be blank)
- keyword - a particular keyword from the tweet (may be blank)
- target - in train.csv only, this denotes whether a tweet is about a real disaster (1) or not
(0)

## Project Outcome
The goal of the project is to build a machine learning model that can accurately predict whether
a tweet is about a real disaster or not. The outcome of the project will be a model that can be
used to classify new, unseen tweets, helping disaster relief organizations and news agencies to
quickly identify tweets that are relevant to disasters.

## Stretch Features
If time persists, some ideas of stretch features are as follow.
- Model tuning: The performance can be improved by tuning the hyperparameters. For
example trying different hyperparameters to see which combination results in the best
performance.
- Preprocessing techniques: Implementing different preprocessing techniques such as
removing stop words, stemming, and handling misspelled words.
- Multilingual classification: The kaggle competition is focused on English language tweets
only. However, expanding the task to include multiple languages could make it more
universal. This would require building a model that can handle multiple languages, which
can require additional preprocessing steps.
