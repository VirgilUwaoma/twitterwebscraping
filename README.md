## twitterwebscraping

Github Link: https://github.com/VirgilUwaoma/twitterwebscraping

### Introduction
The primary objective of this project was to extract data (from anywhere), preprocess and analyze it using python language. We have used an open source library in python called *tweepy* to extract twitter data from the twitter API. There is colossal amount of data available on twitter to extract, but we have chosen a specific topic to perform our analysis on. As the rising housing crisis in Ireland, we decided to extract tweets that contained the keywords - housing/housing crisis/rent and we set the API to only extract tweets from Ireland.

There are many attributes that gets returned as a response in the pull request, we selected the most relevant features for the analysis. They were:
- id
- created_at
- username
- tweet
- retweet_count
- favorite_count
- user_location

The data retrieved was stored in a pandas dataframe and some basic preprocessing on it was performed. We converted the created_at date to the desired (YYYY-MM-DD) format and cleaned the tweet, like removing the links, special characters, punctuations, etc. This preprocessed data was then inserted into a local MYSQL database and retrieved again to perform analysis.

Finally, we worked on 6 critical questions that can be analyzed with this data.
1. What were the words that appeared most frequently in all tweets?
2. What were the most frequent words in tweets from 5 cities/counties with highest number of tweets?
3. Which 10 cities/counties had the maximum number of tweets?
4. How many tweets were posted each day in a week?
5. Which tweet had the maximum retweet count and are there any other tweets from the same username?
6. Which tweet had the maximum favorite count and are there any other tweets from the same username?

The analysis process included: tokenizing & lemmatizing of tweets, removing of stopwords, grouping user location by city or county, making a wordcloud, visualizing different plots, and answering other questions. TPython libraries like nltk, pandas and matplotlib were used in the process of analyzing and visualizing the data.

### Chirag's individual contribution

### Chukwuebuka's individual contribution

### Dipanshu's individual contribution