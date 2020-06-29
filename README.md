# Data Wrangling and Exploration of "WeRateDogs" Twitter data.

## Dataset
My goal for this project is to wrangle WeRateDogs Twitter data to create
analyses and visualizations. WeRateDogs is a Professional Dog rating service
which rates people's dogs with a humorous comment about the dog. Using Python
and its libraries, I have gathered data from a variety of sources and in a
variety of formats, to assess its quality and tidiness, then clean it.
I have gathered data from 3 sources:
1> Twitter archive shared by WeRateDogs, that was downloaded from their Twitter
archive. This archive contains basic tweet data (tweet ID, timestamp, text, etc.)
for 2356 tweets in a csv file - twitter-archive-enhanced.csv
2> Tweet image predictions in a tab separated value file. This file contains
predictions about what breed of dog (or other object, animal, etc.) is present
in each tweet image according to a neural network that can classify breeds of
dogs. The file contains image predictions (the top three only) alongside each
tweet ID, image URL, and the image number that corresponded to the most
confident prediction (numbered 1 to 4 since tweets can have up to four images) -
img_predictions.tsv
3> Retweet count and favorite ("like") count for each tweet in the WeRateDogs T
witter archive. I queried the Twitter API for each tweet's JSON data using
Python's Tweepy library and built a Pandas dataframe using the tweet ID,
retweet count, and favourite count.

## Summary of Findings

In the exploration, I found that the source that people use the most while
tweeting about WeRateDogs is by far the twitter app for the iPhone.
I also found that if you want your dog to get the most likes and retweets, you
need to post a video instead of just a picture. All the top 3 dogs with the most
retweets have their videos posted instead of just a picture and the same goes for
2 out of the top 3 most favourited dogs.
The most common dog name by the data from WeRateDogs is - "Charlie" and "Lucy"!
Both were found to be equally present in the WeRateDogs data.
I also had access to some predictions made by a neural network program which
tried to predict the breed of a dog using its picture. As per my analysis,
the neural network program can accurately predict the breed of the dog 67.73%
of the time. Watch out humans the machines are coming to take over the world!
Finally, I found that unsurprisingly Sunday is the day that most tweets were
created but surprisingly Saturday is the day that least tweets were created!


## References
https://medium.com/ibm-data-science-experience/markdown-for-jupyter-notebooks-cheatsheet-386c05aeebed
