# 202FinalProject
## Project Goal
Problem: Can we train a GPT-2 model to learn gamer slang (gamer girls) and create a twitter bot with it. Can GPT-2 models be able to parse out the nuances of cultural differences, and not just racial bias

### Goals
1. Sentiment Analysis - Download and analyze sentiment expression in tweets by popular gamers and within popular gaming hashtags
Analyze for valence
2. Twitterbot - Create a Twitterbot to tweet our tweets generated by a GPT-2 model that learned on positive tweets

## Downloading Tweets
Using the repository from \minimaxir we were able to download the tweet archives of two users, Pokimane and Lilypichu

## Sentiment Analysis
  * downloaded Tweets from prominent gamer twitter accounts (Ninja, Pokimane)
  * Analyzed these tweets for sentiment
  * Trained a recurrent neural network classifier with 800,000 labeled tweets
  * Used this model to separate the positive and negative tweets

## Generating Tweets
Using a GPT-2 Model we:
  * Learned on tweets from Game Twitter Personalities
  * Used existing GPT-2 Google Colab model
  * Input a single-column csv
  * Used a 124M “small” model
  * Carried out 2000 steps, temperature of .7
  * Generated a .txt file of 1000 tweets at a time

## Creating a Twitterbot
Using [Tracery](https://www.tracery.io/), we were able to create a [bot]https://twitter.com/Magikarmen) to tweet out our generated tweets
  * Created “bot” Twitter Account
  * Set to tweet every 6 hours
  * Created set of rules to generate game-related Tweets
  * Two types: human created (by us) and GPT-2 generated
