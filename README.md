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
As a team member, my contribution involved connecting to the Tweepy API and pulling tweets related to the topic of interest. Connecting to the API required thorough research to understand the data sources and query parameters that could help us obtain relevant tweets.
Once we pulled the tweets, the location column was cleaned to ensure data consistency and was crucial in preparing the data for analysis and visualization.
After cleaning up the data, we visualized it using a word cloud to show the most frequent words in the tweets from the top five counties to provide a quick and easy way to identify the key themes and sentiments expressed in the tweets.
Furthermore, using a bar chart, we visualized the number of tweets from the top 10 counties, and it provided a more comprehensive overview of the distribution of tweets across different locations, helped us identify the areas where discussion about the topic was prevalent, and provided insights into the geographic distribution of public opinion.
Overall, these formed the foundation for further analysis and interpretation by the team.

### Dipanshu's individual contribution

The project involved implementing a database management system where a local connection was established to the database. Data was then obtained from an API and processed to ensure it is clean and relevant. The cleaned data was then inserted into the database using the established connection.

Further, in the project, a specific column in the database named "tweet" was processed using tokenization, lemmatization, and word cloud techniques. Tokenization involves breaking down sentences or phrases into smaller units or tokens to enable easier analysis. Lemmatization, on the other hand, involves converting words to their base or root form to enhance analysis. Word cloud techniques help to visualize frequently occurring words or phrases in a particular text corpus, making it easier to identify significant patterns and trends.

In the analysis section, the project involved extracting and processing data from the database using various techniques and tools. Specifically, the project aimed to identify the maximum number of tweets based on user location. This analysis involved using data manipulation tools to extract relevant information from the database, such as user location and the number of tweets associated with each location. The extracted data was then analyzed using statistical techniques to identify the location with the highest number of tweets.

In this project, the database was managed starting from establishing a connection to the database. After establishing a local connection, the data obtained from an API was cleaned and inserted into the database. Later, the tweet column was tokenized, lemmatized and analyzed using word cloud techniques. In the analysis section, the maximum number of tweets was analyzed based on user location. This involved extracting and processing data from the database using various techniques and tools.