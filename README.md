# cs4412-project-Collin

Project Overview
The aim of this project is to uncover patterns or natural grouping characteristics that lie within Spotify audio feature metadeta, sourced through the official Spotify Web API.
Instead of linking song characteristics to popularity, the study will aim to use learning and association rule mining techniques to find how these musical characteristics given within the data interact and to use
those findings in creating "mood profiles" and discovering track anomalies.

Dataset
Source: Spotify Audio Features (Kaggle) https://www.kaggle.com/datasets/tomigelo/spotify-audio-features?resource=download
This dataset is metadata scraped from the official Spotify Web API. It has around 130,000 tracks and includes attributes for each such as danceability, energy, loudness, speechiness, acousticness, instrumentalness, and valence.

Discovery Questions
Mood Profiles: Are tracks with a high relationship between energy, valence and acousticness able to mathematically be clustered into specific muscial ""moods"?
Feature Co-occurrence: I will be finding a number of track feature co-occurances but an immediate example would be: Do combinations of high amounts of instrumentalness coincide specific tempo ranges in low-speechiness tracks?
Anomalous Track Profiles: What tracks do not align with established and evidenced mood profiles? A hypothetical example would be a track with high energy and low loudness.

Team:
Collin Knowles

M2 Update:
This initial phase of exploratory analysis has shown a number of patterns that give an idea
how to approach the mining phase of this project.
• Strong Feature Correlations: A high positive correlation (0.77) was found between
Loudness and Energy, while there was a significant negative correlation (-0.71 between
acousticness and energy.
• Data Density: Early scatter plots showed that Valence amd energy had a dense, over-
lapping distribution across all features. This confirmed that algorithmic clustering is
helpful in distinguishing "mood profiles", beyond just regular listener intuition.
• Feature Skew: Attributes such as Instrumentalness skewed strongly towards zero, which
indicates that, at least within this dataset, the majority of tracks were voacl-centric
tracks.

The Elbow Method was used to determine k = 4 as the optimal number of clusters. The
rate of decrease in inertia leveled off substantially at this point. Four "Mood Profiles" were
discovered. Each Profile is identified by it’s mathematical center:

• Cluster 0 (Upbeat/High Energy): Representative of positive sounding music. High
valence suggests the music here contains an optimistic tone, that it’s easy dance to and
reminiscent of modern Pop.
• Cluster 1 (Chill/Acoustic Folk): The most distinct of all profiles generated, it shows a
strong inverse relationship in accousticness and energy. Representative of tracks that
are "unplugged" and lower tempo.
• Cluster 2 (Intense / Modern Rock): Energetic but not happy music sonically, this
grouping contained music with more serious tones. It includes most tracks where high
intensity isn’t associated with a positive mood.
• Cluster 3 (Vocal heavy/ Hip Hop): Contains tracks that are on average 5x more wordy
than the other groups. Groups music that is high in wordiness, which encompasses
rap/hip hop that is performed on top of instrumentation
