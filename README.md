# how-do-people-really-feel

# Overview

This project analyses a set of tweets. This specific dataset, from Kaggle, has been critisised for being poorly labelled, so in this project I apply Non-Negative Matrix Factorization (NMF) for topic modeling and VADER for sentiment analysis, aiming to explore patterns and relationships in the data without relying on labels.

The primary goal is to uncover underlying topics within the tweet dataset and analyze how sentiment varies across these topics. This is interesting as it gives a 2D mapping perspective on the sentiment across the ~7300 tweets in the dataset. Given content recommendation algorithms select the content we see, such mappings can be very useful to visualise objectively how likely people are to express a certain sentiment or otherwise, and how this changes between topics. This could have practical uses in industry, for example, uploading datasets containing all posts during a certain day, to compare the sentiment users think people have based on their feeds, versus the one that is in actuality being communicated post-wise.

# Data

Dataset: Kaggle's "Twitter Entity Sentiment Analysis" dataset.
Size: ~7,300 tweets.
Text: Contains user tweets.
Sentiment labels: Given labels, including categories like positive, negative, and neutral. These are not used for model training.

# Approach

Preprocessing: Cleaning the tweets by removing URLs, mentions, hashtags, and stopwords.
Exploratory data analysis (EDA): Exploring word frequencies, tweet lengths, and common topics using visualisation.
Topic modelling: Applying NMF to identify the dominant topics in the tweets.
Sentiment analysis: Using VADER to assign sentiment intensity scores to each tweet.
Clustering and visualisation: Using t-SNE and UMAP for dimensionality reduction and clustering to group tweets based on topic and sentiment intensity.

# Results

- Topic modelling with NMF revealed distinct themes within the dataset.
- Sentiment analysis using VADER provided a nuanced view of sentiment intensity.
- The visualisation techniques showed clear clusters, allowing us to see how topics and sentiments group together across the dataset.

The results show clear topic clusters with varying sentiment distributions. The findings demonstrate how sentiment shifts between topics and how tweets that may appear neutral in tone may contain underlying strong sentiments. VADER sentiment analysis provided insights into sentiment polarity and intensity. The sentiment distribution indicated a heavy concentration of neutral tweets, typical of online discourse, but distinct patterns emerged for more polarised sentiments. For example, some topics, such as topic 3, leaned heavily positive, while others, like topic 9, carried more negative sentiment. These findings reveal that certain subjects provoke stronger emotional responses on Twitter. This could be a very interesting starting point for a variety of subsequent studies, for example, looking into the proliferation patterns of topics based on the different sentiments they carry. 




