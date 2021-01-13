# Song Recommendation System

<p align="center">
  <img width="460" height="300" src="https://github.com/hilmikilickaya/song-recommendation/blob/master/img/SongRecommender.jpg">
  </p>
  
  ## Motivation
  When I was a kid one of the things I enjoyed was playing with the CD player and making a list of my favorite songs. In the 90’s most of us couldn't imagine that we would be accessing hundreds of thousands of songs with one click. Let alone that, apps could recommend different songs based on our preferences and playlists using machine learning. One of the most used machine learning algorithms is recommendation systems. I just wanted to go back and play my favorite childhood game in a different way. Not only listening and creating my playlist but creating my own recommender system to find my favorite songs.  In my project, I created a recommender system with different features to compare them. I used cosine similarity to find similarities between the songs.
  
  ## Content Base Recommender
  *Content-based methods* gives recommendations based on the similarity of two song contents or attributes. 

 **Content-based methods** are computationally fast and interpretable. Moreover, they can be efficiently adapted to new items or users. 
However, one of the biggest limitations of content-based recommendation systems is that the model only learns to recommend items of the same type that the user is already using or listening to.
  
  
  ## Data
  
  I got the data from [kaggle](https://www.kaggle.com/imuhammad/audio-features-and-lyrics-of-spotify-songs). The dataset contains over 18 thousand songs from 6 thousands artists and also has Spotify audio features (accousticness, instrumentalness, danceability etc.) , and lyrics.
  <p align="center">
  <img width="460" height="500" src="https://github.com/hilmikilickaya/song-recommendation/blob/master/img/genre.png">
  </p>

  ## Tf-idf 
  TF-IDF is a statistical measure that evaluates how relevant a word is to a document in a collection of documents. This is done by multiplying two metrics: how many times a word appears in a document, and the inverse document frequency of the word across a set of documents.
  
  <p align="center">
  <img width="460" height="300" src="https://github.com/hilmikilickaya/song-recommendation/blob/master/img/lessbins_doc.png">
  </p>
  
  | Recommendations for Lady Gaga - Just Dance  |
  | --------------------------------------------|
   The Black Keys - Howlin’ For You
Heaven 17 - Let Me Go
Dada Life - Feed The Dada 
The Cranberries - When You’re Gone
Louis Futon - Rewind 
Glen Campbell - Southern Nights 
Amber - This Is Your Night
Little Mix - Hair
Billie Eilish - 8 


  ## LDA 
  Topic modeling is a type of statistical modeling for discovering the abstract “topics” that occur in a collection of documents. Latent Dirichlet Allocation (LDA) is an example of topic model and is used to classify text in a document to a particular topic. It builds a topic per document model and words per topic model, modeled as Dirichlet distributions. I used 10 topics for my model.
  
  <p align="center">
  <img width="900" height="400" src="https://github.com/hilmikilickaya/song-recommendation/blob/master/img/topicwords.png.png">
  </p>
  
  | Recommendations for Lady Gaga - Just Dance  |
  | --------------------------------------------|
   Coko - Endow Me
Peach Pit - Peach Pit 
Chico DeBarge - Iggin’ me
Latimore - Let’s Straighten It Out
Taylor Swift - ME!
Fire From The Gods - Right Now 
The Smiths - The Boy with the Thorn in His Side
Joe Public - Do You Everynite
YUNGBLUD - Original me 

  
  ## Audio Features
   Spotify has audio features, which include danceability which tells how suitable a track is for dancing based on a combination of musical elements, accousticness tells whether a track is acoustic or not and instrumentallness predicts whether a track contains vocals. I used audio features to find cosine similarities between the songs. 

  | Recommendations for Lady Gaga - Just Dance  |
  | --------------------------------------------|
   Kesha - Die Young
Jacala - Bottles  
Hillsong Young & Free - This Is Living
Jones Brothers - Sucker
Garbage - Stupid Girl
COIN - Cemetery  
Hedley - In Love with A Broken Heart
Alice Smith - Fool For you
Smallpools - Million Bucks

  
  ## Audio Features + LDA
  | Recommendations for Lady Gaga - Just Dance  |
  | --------------------------------------------|
   Kesha - Die Young
Jones Brothers - Sucker 
Hillsong Young & Free - This Is Living
Alice Smith - Fool For you
Garbage - Stupid Girl
Jacala - Bottles 
P!nk - Can We Pretend
Garbage - Only Happy  When It Rains
The Used - Cry



## Going Forward
I would like to collect more data using Spotify API to feed my model, and also I would like to get users data to create a collabaritive recommender system. My CPU doesn't have enough memory to carry out heavy computation tasks like cosine similarities. In the future, I would like to utilize AWS cloud computing services to carry out these tasks. 
