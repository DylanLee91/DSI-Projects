# Capstone Project

# Executive Summary
Sports fans generate a great deal of opinionated data in response to what is happening during various sporting events. In this data there are both discrete topics and sentiments associated with each topic. To investigate the ability of NLP to model and provide insights on collected social media sentiment, I tested this by collecting and examining topics and sentiment during a specific football event. The data was cleaned to leave only basic english characters and words stripped of stopwords, lemmatized, and tokenized. The tweets were then assigned a sentiment score based on the tokens identified, before they were run through an unsupervised latent Dirichlet allocation model to identify and assign topics to the tweets. 
The results do provide insight into fan sentiment during the chosen event and that my approach was effective in answering the initial problem statement

# Problem Statement
How can we use social media as an aggregator of topics and sentiment in user discussions? To investigate this, I used tweets posted over the course of a real time event and checked to see how sentiment and topics occurrence changed in response to discrete smaller events over the period.

### Topic Modeling

https://towardsdatascience.com/twitter-topic-modeling-e0e3315b12e2

https://towardsdatascience.com/latent-dirichlet-allocation-lda-9d1cd064ffa2

https://radimrehurek.com/gensim/models/ldamodel.html

### Sentiment Analysis with Vader
https://blog.quantinsti.com/vader-sentiment/#:~:text=Compound%20VADER%20scores%20for%20analyzing,1%20(most%20extreme%20positive)

https://towardsdatascience.com/almost-real-time-twitter-sentiment-analysis-with-tweep-vader-f88ed5b93b1c

https://towardsdatascience.com/sentimental-analysis-using-vader-a3415fef7664

https://github.com/cjhutto/vaderSentiment

Hutto, C.J. & Gilbert, E.E. (2014). VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text. Eighth International Conference on Weblogs and Social Media (ICWSM-14). Ann Arbor, MI, June 2014.

### Visualisation

https://towardsdatascience.com/visualization-of-information-from-raw-twitter-data-part-1-99181ad19c

## Scraping

### Tweepy

https://www.storybench.org/how-to-collect-tweets-from-the-twitter-streaming-api-using-python/

https://dzone.com/articles/stream-tweets-the-easy-way-in-under-15-lines-of-co

https://medium.com/@jaimezornoza/downloading-data-from-twitter-using-the-streaming-api-3ac6766ba96c

http://docs.tweepy.org/en/latest/streaming_how_to.html

https://medium.com/@adam.oudad/stream-tweets-with-tweepy-in-python-99e85b6df468

https://towardsdatascience.com/selenium-tweepy-to-scrap-tweets-from-tweeter-and-analysing-sentiments-1804db3478ac

https://towardsdatascience.com/how-to-scrape-more-information-from-tweets-on-twitter-44fd540b8a1f

### Praw scraping

https://praw.readthedocs.io/en/latest/getting_started/configuration.html#configuration

https://www.storybench.org/how-to-scrape-reddit-with-python/

https://medium.com/analytics-vidhya/praw-a-python-package-to-scrape-reddit-post-data-b759a339ed9a

https://towardsdatascience.com/scraping-reddit-data-1c0af3040768

https://www.reddit.com/r/redditdev/comments/77z44v/praw_get_timestamp_from_comment_stream/

### Match timing references

https://www.theguardian.com/football/live/2020/oct/04/aston-villa-v-liverpool-premier-league-live?page=with:block-5f79f7378f08abd321a6cc45#liveblog-navigation

https://www.theguardian.com/football/live/2020/oct/04/manchester-united-v-tottenham-premier-league-live

https://www.theguardian.com/football/live/2020/oct/03/chelsea-v-crystal-palace-premier-league-live