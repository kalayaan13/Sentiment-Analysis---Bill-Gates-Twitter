# Sentiment Analysis for Bill Gates' Twitter

Bill Gates is one of the wealthiest influential personalities in the world and co-founded Microsoft, the world's largest personal computer software company. He uses Twitter frequently and shows his personality and influence on the worldwide cause.

The project is for determining how positive, negative, or neutral using his recent 100 tweets from his Twitter Account @BillGates. The data is collected using the Twitter API and Sentiment Analysis to find information about his tweets.

## Data Collection

**Tweepy** library was used to access Twitter API and extract the recent 100 tweets from Bill Gates' Twitter profile. The API authentication keys are secured in the config.ini file and accessed using configparser.

## Data Preparation

**Pandas** library was used to store the data into pandas DataFrame for easier data manipulation.

## Data Cleaning

**Regular Expression** or **re** module was used for cleaning the tweets by removing the username, '#' character, retweet, and website link.

## Sentiment Analysis 

**Text Blob** library was used for determining the subjectivity and polarity score for every tweet.

The **subjectivity score** depends on how opinionated the tweet is. The score ranges from 0 to 1, on which the closer the score gets to 1, the tweet is being considered subjective. On the other hand, if the score is closer to 0, then the tweet is considered objective or factual. 

The **polarity score** refers to how positive, negative, or neutral the tweet is. The range of the polarity score is from -1 to 1. 

Positive : score > 0

Neutral : score = 0 

Negative : score < 0

### Word Cloud

The Word Cloud determines the frequent words used in his tweets collected. The larger the font size, the more Bill Gate uses it. The image shows a bag of words that are usually words like "Thank", "Congrats", "better", and etc., which referred that he is tweeting with positive words.

![wordcloud](https://user-images.githubusercontent.com/80330171/174859270-25152b4d-b129-40b3-b24d-4d03e8c530d0.png)

### Scatter Plot

To visualize the data which shows the relationship of the score between the subjectivity and polarity score. The plot shows a correlation relationship between the subjectivity score and polarity score a **moderate**, **positive**, and  **linear**.
![Polarity_vs_Subjectivity](https://user-images.githubusercontent.com/80330171/174859282-23db6b3c-11ce-4458-9489-968ae61e4034.png)

### Bar Graph

To visualize the counts of tweets considered being positive, negative, and neutral from the 100 tweets collected. The graph shows that the mostly the tweets are positive.

![Sentiments_vs_Counts](https://user-images.githubusercontent.com/80330171/174861069-b26ba072-5db9-40bc-a6fc-907335001317.png)


# Conclusion

Based on the observations from the three visualizations, Bill Gates' tweets shows optimism and express gratitude on most of his tweets. 
