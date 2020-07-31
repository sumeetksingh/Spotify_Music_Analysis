# Spotify_Music_Analysis
Summary

Music industry has revolutionized since the start of streaming services. Spotify is a top streaming service with over 50 million tracks and 280 million monthly active users. We have already seen how personalized recommendation has brought millions in users and profits to the company. Algorithms like Collaborative Filtering started the rise of using Machine learning to help personalize content for users on streaming platforms. The objective of this paper is a little different, we want to see what constitutes for a “Hit” or “Flop” song on Spotify, we will also try to predict if a song is “Hit” or “Flop” using various algorithms and finally, we will recommend older songs based on the audio features of current “Hit” songs. We used Accuracy to evaluate the performances of our models. We found one algorithm stood out more than the rest and Instrumentalness is a feature that makes a song “Hit” or “Flop”  and in the end, We recommended some old songs that has audio features of current “Hit” songs.


1)	Introduction

Spotify allows users to scrape data and audio features for each of its tracks, in our dataset we have audio features from various kinds of music and of different years. Since music changes so rapidly, we will see over the years what has been a factor in making a song “Hit” or “flop”. We will generate a classifier to predict outcomes(“Hit/Flop”) and other algorithms to help us deduce what features make a “Hit” or “Flop” song on Spotify and in the end, we will generate a list of Old songs which are similar to the current “Hit” songs.

2)	Data Description

"Spotifydata.csv" is the dataset with the latest tracks and its audio features and “dataset_of_00s” and “dataset_of_10s” are datasets with older tracks from Years 2000’s and 2010’s. We have combined the “dataset_of_00s” and dataset_of_10s” into one dataset. The datasets have 17 columns related to a song’s features such as mode, key, etc. The Spotifydata.csv has an additional column known as “target” where the value is 1 if “Hit” and 0 for “Flop”. (Read more about the features here: https://developer.spotify.com/documentation/web-api/reference/tracks/get-audio-features/) 

3)	Goal

There are three main objectives we want to achieve from the project
1)	We want to able to classify if a Song is “Hit” or “Flop”.
2)	We want to quantify the importance of the audio features and how it affects in classifying a “Hit” or “Flop” song.
3)	We want to recommend “Hit” songs from the past based on the audio features of “Hit” songs of the present.

4) Conclusion

We used Random Forest to classify the songs and we saw It is easier to predict “Hit” songs of the past than the present based on its audio features. 
We had 79% accuracy while predicting the outcome of latest music. Whereas 86% accuracy while predicting the outcome of older music.
Most important audio feature from songs from the past or present is Instrumentalness of the music. We also found list of old songs that may have similar audio features to the present “Hit” songs.
