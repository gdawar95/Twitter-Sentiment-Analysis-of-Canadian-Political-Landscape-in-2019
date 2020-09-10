# Twitter-Sentiment-Analysis-of-Canadian-Political-Landscape-in-2019

The goal is to essentially use sentiment analysis on Twitter data to get insight into the 2019 Canadian elections

## Background
Sentiment analysis is a technology of increasing importance in the modern society as it allows individuals and organizations to detect trends in public opinion by analyzing social media content. Keeping abreast of socio-political developments is especially important during periods of policy shifts such as election years, when both electoral candidates and companies can benefit from sentiment analysis by making appropriate changes to their campaigning and business strategies respectively.

## Data Insights
The Sentiment.csv file contains 130K+ labeled generic tweet texts. It had their sentiments already analyzed and recorded as: positive or negative. Each line is a single tweet, which may contain multiple sentences despite their brevity. The fields of each line are:
1. sentiment can be “positive” or “negative”
2. text the text of the tweet

The second data set, Canadian_elections_2019.csv, contains a list of tweets regarding the 2019 Canadian elections. The fields of each line are:

0. sentiment can be “positive” or “negative”
1. negative_reason reason for negative tweets. Left blank for positive tweets.
2. text the text of the tweet

Both datasets have been collected directly from the web, so they may contain html tags, hashtags, and user tags.

# INDEX of Notebook

### 0.	NOTEBOOK PREPARATION
    0.1	IMPORTING LIBRARIES
    0.2	DEFINING FUNCTIONS
### 1.	DATA PREPARATION
    1.1	Checking for null values
    1.2	Cleaning the tweets
### 2.	DATA EXPLORATION
### 3.	MODEL PREPARATION ON SETIMENTS.CSV
    3.1	Trying multiple classification algorithms with hyper parameter tuning and cross val.
        3.1.1	Logistic regression with hyp. param. tuning
        3.1.2	k-NN with hyp. param. tuning
        3.1.3	Naive Bayes with hyp. param. tuning
        3.1.4	SVM with hyp. param. tuning
        3.1.5	decision trees with hyp. param. tuning
        3.1.6	Random Forest with hyp. param. tuning
        3.1.7	XGBoost with hyp. param. tuning
    3.2	Analysing the accuracy results of all the models

### 4.	MODEL IMPLIMENTATION ON ELECTIONS
    4.1	TF on Election Dataset
    4.2	General tweet Model Implementation and testing on Election Dataset
    4.3	Prediction Results Exploration
### 5.	MODEL IMPLIMENTATION ON ELECTIONS TO CLASSIFY 'NEGATIVE REASON' OF ELECTION TWEETS
    5.1	Exploring the negative reasons
    5.2	Combining negative reason Categories
    5.3	Implementing classification models
### 6.	RESULTS
### 7.	BONUS
    7.1	Using Word2Vec Model instead of TF (Bag of Words)
        7.1.1 Implementing All the classification models with w2v (Logistic Regression, SVM, decision tree, random forest, XG Boost)
    7.2	Implementing N-Grams in Bag of Words and TF IDF
        7.2.1	Implementing All the classification models with N-Grams (Logistic Regression, SVM, decision tree, random forest, XG Boost)
        7.2.2	Implementing Log reg general model with ngrams on elections data set
