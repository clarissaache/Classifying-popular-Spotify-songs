# Classifying-popular-Spotify-songs
Classifying popular songs from Spotify using parametric and non-parametric models

In this analysis, I would explored how different features of popular songs can determine the music genre that a song belongs to using parametric (multinomial logistic regression model) and non-parametrics models (tree based machine learning models). 
Music genres seem like arbitrary categories that identify songs as belonging to a certain style or convention. I believe as new music is created, genre limits become less obvious, and the genres themselves become less and less objective classifiers. Spotify warns the users of their API about the very obscure genres and sub-genres that they had to include for their less represented newer music styles.
I will focus in the most common genres (pop, rap, rock, latin, EDM, and R&B), and a mix of older and newer songs.

There are 12 audio features for each track, including confidence measures like acousticness, liveness, speechiness and instrumentalness, perceptual measures like energy, loudness, danceability and valence (positiveness), and descriptors like duration, tempo, key, and mode. A full data dictionary can be found in the Spotify API site.

[Previous work] (https://www.kaylinpavlik.com/classifying-songs-genres/) has been done using decision tree, random forest, and XGBoost models producing the following conclusions. 
"The random forest model was able to classify ~54% of songs into the correct genre, while the individual decision tree shed light on which audio features were most relevant for classifying each genre:
Rap is speechy. Rock, you can’t dance to it. EDM has high tempo. R&B makes long songs. Latin is very danceable. Pop is everything else, hard to describe."

My analysis will try to reproduce these outcomes but using a lower-level regression model (which will probably not be as good) and some other better-performing models to predict the genre classification.
