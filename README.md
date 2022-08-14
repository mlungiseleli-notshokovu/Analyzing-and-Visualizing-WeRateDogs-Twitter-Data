#Udacity's Data Analyst Nanodegree Program
# Analyzing-and-Visualizing-WeRateDogs-Twitter-Data
_2nd project for the Data Analyst Nanodegree from Udacity_

The **WeRateDogs** Twitter archive
I was given this file  _**twitter_archive_enhanced.csv**_ to download manually by clicking the following link: 'https://d17h27t6h515a5.cloudfront.net/topher/2017/August/59a4e958_twitter-archive-enhanced/twitter-archive-enhanced.csv'. 
Once it was downloaded, I uploaded it and read the data into a pandas DataFrame.

The tweet image predictions
This file (**image_predictions.tsv**) is present in each tweet according to a neural network. It is hosted on Udacity's servers and was downloaded programmatically using the Requests library and the following URL: https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv

Additional data from the Twitter API
I Gather each tweet's retweet count and favorite ("like") count at the minimum and any additional data I found interesting. Using the tweet IDs in the WeRateDogs Twitter archive, I queried the Twitter API for each tweet's JSON data using Python's Tweepy library and stored each tweet's entire set of JSON data in a file called **tweet_json.txt**.

Each tweet's JSON data was written to its own line. I then read this **.txt** file line by line into a pandas DataFrame with (at minimum) tweet ID, retweet count, and favorite count
