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
I organized the 12 groups into 3 generations and applied K-Means Clustering to group their songs into 3 clusters. To determine the optimal number of clusters among 2 to 10 options, I used the silhouette method. Furthermore, I decided to visually represent the connection between popularity and individual audio features. I obtained cluster plots by combining all the songs from all generations.

The results of the clusters reveal a lack of distinct groups, as the data points are scattered across the plots. It appears that there is no evident correlation between a song's popularity and its audio features. This suggests that further analysis is required to accurately determine the factors contributing to a song's popularity in K-pop. It is important to recognize that the popularity of a song involves more than just its music, indicating that additional aspects should be taken into consideration for a comprehensive understanding.

Here are the cluster plots:
![all gen - clustering acousticness](https://github.com/aaryasaheed/Final-Project/assets/130434126/a9c8b0bb-ae36-4f84-bcfc-a62f2f5dc3ab)
![all gen - clustering danceability](https://github.com/aaryasaheed/Final-Project/assets/130434126/afb6c42a-5780-449c-8479-899946f9a47c)
![all gen - clustering energy](https://github.com/aaryasaheed/Final-Project/assets/130434126/60c9e1a2-5601-4e07-bc20-4ad3ee517a53)
![all gen - clustering liveness](https://github.com/aaryasaheed/Final-Project/assets/130434126/a27966bc-5cd6-48cb-a16e-2b5669e44953)
![all gen - clustering loudness](https://github.com/aaryasaheed/Final-Project/assets/130434126/02f50764-5186-4d3c-8f25-e9a12cdd5d08)
![all gen - clustering speechiness](https://github.com/aaryasaheed/Final-Project/assets/130434126/f1802b24-b928-4b14-a2de-62a67cbd15a0)
![all gen - clustering tempo](https://github.com/aaryasaheed/Final-Project/assets/130434126/9e5fe436-252c-4760-8d96-ef193132ee0e)
![all gen - clustering valence](https://github.com/aaryasaheed/Final-Project/assets/130434126/27364601-b711-40b8-8dd6-e5c1936fb5fa)


I then created scatterplots for all the songs across generations and used different colors to represent each generation. This visual representation revealed a clear distinction where the second generation appeared to have a lower level of popularity compared to other generations. This finding suggests that a song's popularity is heavily influenced by the personal taste of fans.

Here are the plots:
![popularity vs acousticness](https://github.com/aaryasaheed/Final-Project/assets/130434126/795970e9-e60e-4ac1-8ae0-b5103c3265d6)
![popularity vs danceabililty](https://github.com/aaryasaheed/Final-Project/assets/130434126/44ff2464-9383-4c99-b7ca-0f110a378129)
![popularity vs energy](https://github.com/aaryasaheed/Final-Project/assets/130434126/36e55ed6-4408-4757-abee-7e731f160d18)
![popularity vs liveness](https://github.com/aaryasaheed/Final-Project/assets/130434126/7037fa3c-f101-485b-ab28-df3d592b0a32)
![popularity vs loudness](https://github.com/aaryasaheed/Final-Project/assets/130434126/bb800a0d-5b16-49a5-ab0c-b8b6d3f9eb94)
![popularity vs speechiness](https://github.com/aaryasaheed/Final-Project/assets/130434126/5ed24bb1-5530-4be9-bcee-b99a696a4064)
![popularity vs tempo](https://github.com/aaryasaheed/Final-Project/assets/130434126/6cd0c2f6-0a67-4d7b-8efd-815241dac45d)
![popularity vs valence](https://github.com/aaryasaheed/Final-Project/assets/130434126/90a9e3b5-158a-454f-b92b-200d6b353af9)







# Mean of Audio Features
By plotting the means of the audio features grouped by generation, I discovered interesting patterns. It became evident that the audio features across generations are quite similar, with only two features showing significant evolution: tempo and loudness. Songs from the fourth generation have a higher tempo and louder volume compared to the other generations. Additionally, energy, danceability, and valence decreased gradually across the generations. However, the remaining features exhibited relatively consistent means.

This observation leads me to believe that the songs produced by older generations were more vibrant and bold, contributing to the uniqueness of K-pop. On the other hand, the newer generations seem to create music that appeals to a broader audience. This shift may be related to the fact that during the second generation, K-pop fans were primarily concentrated in Asian countries. Today, however, K-pop has achieved global recognition and popularity, suggesting a need for music that resonates with a wider range of listeners.

Here are the plots:
![mean of tempo by generation](https://github.com/aaryasaheed/Final-Project/assets/130434126/eb015afb-8de0-480b-93fd-0f02f802895d)
![mean of audio features by generation](https://github.com/aaryasaheed/Final-Project/assets/130434126/8ccf03da-bc6a-4057-8fba-7a1cdc0c9e89)

# Track Statistics
Average Track Duration: There is a noticeable decrease in the average track duration across generations. The second generation had the longest average track duration (218.132 seconds), followed by the third generation (198.837 seconds), and the fourth generation (186.647 seconds). This suggests a shift towards shorter songs over time. 

These findings indicate a shift in focus within the newer generation of K-pop songs. The songs from the newer generation appear to prioritize creating viral moments and dance challenges on social media platforms. These shorter and impactful tracks are designed to capture attention and engage listeners in a dynamic and interactive manner. In contrast, the older generations of K-pop seem to have placed a greater emphasis on the songs themselves, placing less emphasis on creating specific viral moments or dance challenges. 

Average Tempo: The average tempo shows a slight increase from the second (117.969 BPM) to the third generation (118.478 BPM​), with the fourth generation having the highest average tempo of 130.610 BPM. This indicates a trend towards faster-paced songs in more recent generations. The increase in average tempo may indicate a shift towards more energetic and fast-paced music, which could align with the industry's focus on dynamic performances and captivating choreography.

# Regression: Predicted VS Actual Popularity
Comparing the Mean Squared Error (MSE) values for predicted versus actual popularity of songs in different generations of K-pop reveals interesting insights:

The MSE for the second generation is 36.36, which is relatively high. This suggests that the linear regression model had a poorer fit to the second generation data, indicating weaker correlation between the selected audio features and the popularity of songs in this generation.

On the other hand, the third generation shows the lowest MSE value of 24.38, indicating a better fit of the linear regression model to the third generation data. This suggests that the selected audio features have a stronger correlation with the popularity of songs in the third generation, enabling more accurate predictions.

The fourth generation has a moderate MSE value of 32.30. While not as low as the third generation, it still suggests a reasonably good fit between the selected features and the popularity of songs in this generation.

Based on the MSE values, it appears that the selected audio features are more relevant for predicting the popularity of songs in the third generation compared to the second and fourth generations. However, it's important to note that these results only provide a partial understanding of the evolution of K-pop across different generations. To fully understand the evolution of K-pop, we need to analyze more, consider other factors, and take a broader approach.

Here are the regression plots:
![regression plot 2nd gen](https://github.com/aaryasaheed/Final-Project/assets/130434126/7a7d3247-4e0d-409b-9580-5d26fbb1ff9e)
![regression plot 3rd gen](https://github.com/aaryasaheed/Final-Project/assets/130434126/d47ff389-84dd-43fc-af29-979e8816ab6f)
![regression plot 4th gen](https://github.com/aaryasaheed/Final-Project/assets/130434126/1b7d98e6-fe49-486f-93ce-d153e6a56a35)

# Further Analysis
I also examined the release dates of top tracks and albums for all the groups. I did not observe any significant patterns across the different generations.

For the second generation groups, there seemed to be an even distribution of releases throughout the months, suggesting no particular preference for specific seasons or months. However, for the third generation, there was a tendency to release more music during the fall. On the other hand, the fourth generation groups appeared to release their music more frequently during the summer and fall months.

This lack of consistent patterns in release dates could imply several things. It is possible that the timing of releases is influenced by various factors, such as promotional strategies, availability of resources, or external market considerations. It indicates that there is no direct correlation between release timing and the popularity or success of songs in K-pop.

I also compared the popularity of the groups based on the popularity score of their top tracks. The analysis revealed that second generation groups generally had lower popularity scores, while the third and fourth generation groups exhibited similar levels of popularity. This finding aligns with the observations from the scatterplots comparing the generations.

Additionally, I plotted the groups based on their follower counts, which highlighted that BTS has the largest number of followers. This emphasizes the immense popularity of BTS within the K-pop industry. However, it's important to note that these plots primarily reflect the personal preferences of fans and may not provide comprehensive insights into other aspects of the groups' success or the overall landscape of K-pop.

To gain a more comprehensive understanding of the dynamics behind popularity and success within the K-pop industry, it would be beneficial to consider various other factors. These could include factors such as album sales, concert attendance, social media engagements, and cultural impact. By analyzing these additional elements, we can paint a bigger picture of the K-pop landscape and the factors contributing to the success and popularity of different groups.

Here are the plots:
![song popularity by artist](https://github.com/aaryasaheed/Final-Project/assets/130434126/8b66305a-01e1-4f2b-8ae1-ef2e84af44ee)
![followers count by artist](https://github.com/aaryasaheed/Final-Project/assets/130434126/f9879994-929a-49a4-b32e-2035bfcfdeb9)

# Conclusion
K-pop, as a music genre, is known to be quite diverse and groups tend to experiment with various genres. As a result, there are no clear distinct differences in audio features across generations, indicating the versatility and flexibility of K-pop as a musical style.

However, one clear distinction that can be found between the generations is how advanced the newer generations are. They are more willing to embrace diversity and take on new challenges, constantly pushing the boundaries of their music and performances. In contrast, the older generations often maintained consistency in their group's concept, showcasing a more established and defined identity.

Over the years, K-pop has experienced significant globalization. Fans from all around the world have shown great interest in the newer groups, leading to a broader international fan base. This expansion of K-pop's reach contributes to the genre's overall success and popularity.

The success of a K-pop group can be attributed to the diversity present within its music and the genre's unique qualities. The ability of K-pop groups to explore different musical styles and concepts sets them apart and appeals to a wide range of listeners. The continuous innovation and creativity within the genre are key factors driving its success and attracting fans globally.
​

# Deployment:
[](https://mybinder.org/v2/gh/aaryasaheed/Final-Project.git/main?labpath=Final_Project.ipynb)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/aaryasaheed/Final-Project.git/main?labpath=Final%20Project.ipynb)](https://mybinder.org/v2/gh/aaryasaheed/Final-Project.git/main?labpath=Final_Project.ipynb)


[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/aaryasaheed/Final-Project.git/main?labpath=Final_Project.ipynb)
.. image:: https://mybinder.org/badge_logo.svg
 :target: https://mybinder.org/v2/gh/aaryasaheed/Final-Project.git/main?labpath=Final_Project.ipynb

 
