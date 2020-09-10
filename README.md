# Twitter-Sentiment-Analysis-of-Canadian-Political-Landscape-in-2019

The goal is to essentially use sentiment analysis on Twitter data to get insight into the 2019 Canadian elections

## Background
Sentiment analysis is a technology of increasing importance in the modern society as it allows individuals and organizations to detect trends in public opinion by analyzing social media content. Keeping abreast of socio-political developments is especially important during periods of policy shifts such as election years, when both electoral candidates and companies can benefit from sentiment analysis by making appropriate changes to their campaigning and business strategies respectively.

## Data Insights
The Sentiment.csv file contains 130K+ labeled generic tweet texts. It had their sentiments already analyzed and recorded as: positive or negative. Each line is a single tweet, which may contain multiple sentences despite their brevity. The fields of each line are:
1 sentiment can be “positive” or “negative”
2 text the text of the tweet

The second data set, Canadian_elections_2019.csv, contains a list of tweets regarding the 2019 Canadian elections. The fields of each line are:
0 sentiment can be “positive” or “negative”
1 negative_reason reason for negative tweets. Left blank for positive tweets.
2 text the text of the tweet

Both datasets have been collected directly from the web, so they may contain html tags, hashtags, and user tags.


