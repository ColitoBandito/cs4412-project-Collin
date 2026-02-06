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
