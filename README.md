## twitterwebscraping

Github Link: https://github.com/VirgilUwaoma/twitterwebscraping

### Introduction
The primary objective of this project was to extract data (from anywhere), preprocess and analyze it using Python language. We have used an open-source library in Python called *tweepy* to extract Twitter data from the Twitter API. There is a colossal amount of data available on Twitter to extract, but we have chosen a specific topic to perform our analysis on. As the rising housing crisis in Ireland, we decided to extract tweets that contained the keywords - housing/housing crisis/rent and we set the API to only extract tweets from Ireland.

There are many attributes that get returned as a response in the pull request, we selected the most relevant features for the analysis. They were:
- id
- created_at
- username
- tweet
- retweet_count
- favorite_count
- user_location

The data retrieved was stored in pandas dataframe and some basic preprocessing on it was performed. We converted the created_at date to the desired (YYYY-MM-DD) format and cleaned the tweet, which involved removing the links, special characters, punctuations, etc. This preprocessed data was then inserted into a local MYSQL database and retrieved to perform analysis.

Finally, we worked on 6 critical questions that can be analyzed with this data.
1. What were the words that appeared most frequently in all tweets?
2. What were the most frequent words in tweets from 5 cities/counties with the most tweets?
3. Which 10 cities/counties had the maximum number of tweets?
4. How many tweets were posted each day in a week?
5. Which tweet had the maximum retweet count and are there other tweets from the same username?
6. Which tweet had the maximum favorite count and are there other tweets from the same username?

The analysis process included: tokenizing & lemmatizing the tweets, removing stopwords, grouping user location by city or county, making a wordcloud, visualizing different plots, and answering other questions. Python libraries like nltk, pandas and matplotlib were used in the process of analyzing and visualizing the data.

### Chirag's individual contribution
My tasks in completing this project included assisting my group members in setting up the API and researching and reading the API documentation for extracting the desired data. The core task to which I contributed was data preprocessing, where I did some basic checks on the raw data using the *pandas* library. This is a crucial step to ensure that the data does not lead to any errors in the future. Then I converted the date to a desired format using the *datetime* library and used string and regex functions to clean the tweet. My previous learnings on text cleaning helped me majorly to complete this task. In the analysis part, I generated the line plot for the number of tweets per day and also worked on the tweet with a maximum retweet and like count. Finally, the introduction part of the project documentation was done by me where I summarized the objective and the whole process of this project.

### Chukwuebuka's individual contribution
As a team member, my contribution involved connecting to the Tweepy API and pulling tweets related to the topic of interest. Connecting to the API required thorough research to understand the data sources and query parameters that could help us obtain relevant tweets.
Once we pulled the tweets, the location column was cleaned to ensure data consistency and was crucial in preparing the data for analysis and visualization.
After cleaning up the data, we visualized it using a word cloud to show the most frequent words in the tweets from the top five counties to provide a quick and easy way to identify the key themes and sentiments expressed in the tweets.
Furthermore, using a bar chart, we visualized the number of tweets from the top 10 counties, and it provided a more comprehensive overview of the distribution of tweets across different locations, helped us identify the areas where discussion about the topic was prevalent, and provided insights into the geographic distribution of public opinion.
Overall, these formed the foundation for further analysis and interpretation by the team.

### Dipanshu's individual contribution
In this project, I helped the team for selecting the best features to extract from the API that would be useful in performing all types of analysis. My prime contribution was to communicate between the database and Python. The tasks involved establishing a local connection with the MySQL database, designing a schema to store the preprocessed data, and inserting and extracting the data from the database. Later, a specific column in the database named *cleaned_tweet* was processed using tokenization and lemmatization. In this process, the tweets are separated word by word into meaningful chunks and are then transformed into their base words to reduce variance and complexity in data. Lastly, I also generated the word cloud for the tweets and visualized the maximum number of tweets based on user location which was later optimized and modified by the team.