# Final-Project

In my project, I do an analysis of the evolution of K-POP across the three more recent generations. 
​
# Introduction
K-pop is a highly popular genre of music that emerged from South Korea. It incorporates various musical styles like hip-hop, electronic dance, jazz, and rock, and is performed by groups consisting of a range of members, from four to as many as 21. ​

Over the years, K-Pop has evolved through four distinct generations, each embodying changes that mirror trends in pop culture, industry dynamics, and aesthetics. These generations encompass various aspects like fashion, concepts, music, and even fan culture. ​

Today, the primary focus will be on the three most recent generations of K-Pop and their evolution. We will explore the similarities and differences in their music, highlighting the changes in audio features and developments that have occurred within these generations. We will also be discussing popularity and release date patterns. ​

The groups I focused on for my analysis are Girls Generation, SHINee, Super Junior, Apink, BTS, SEVENTEEN, TWICE, EXO, LE SSERAFIM, ENHYPEN, NewJeans and ATEEZ. 

# Objectives

* Visualize trends in popularity of top tracks by some K-POP groups relative to audio features​
* Analysis of release dates ​and popularity
* Give insights into the evolution of K-POP across three generations
​
# Data Collection
Used Spotify's Web API to extract songs and albums information from the groups and their features. Each song had the following features:
* Song Name
* Artist
* Album
* Track ID
* Acousticness
* Danceability
* Duration
* Energy
* Liveness
* Loudness
* Speechiness
* Tempo
* Time Signature
* Valence

## Clustering
I divided the 12 groups into 3 generations and then grouped the groups' songs into 3 clusters using K-Means Clustering. I used the silhouette method to determine the number of clusters that would give me the best results out of the possibility of 2 to 10 clusters. 
Here are the cluster plots I got when I clustered all the songs from all generations together:
![Cluster Plots (All gen](all gen - clustering acousticness.png)
![all gen - clustering acousticness](https://github.com/aaryasaheed/Final-Project/assets/130434126/a9c8b0bb-ae36-4f84-bcfc-a62f2f5dc3ab)






# Deployment:
[](https://mybinder.org/v2/gh/aaryasaheed/Final-Project.git/main?labpath=Final_Project.ipynb)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/aaryasaheed/Final-Project.git/main?labpath=Final%20Project.ipynb)](https://mybinder.org/v2/gh/aaryasaheed/Final-Project.git/main?labpath=Final_Project.ipynb)


[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/aaryasaheed/Final-Project.git/main?labpath=Final_Project.ipynb)
.. image:: https://mybinder.org/badge_logo.svg
 :target: https://mybinder.org/v2/gh/aaryasaheed/Final-Project.git/main?labpath=Final_Project.ipynb

 
