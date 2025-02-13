# Movie Recommendation System

This project is a movie recommendation system built with Streamlit and powered by a machine learning model. It recommends movies based on a selected title using cosine similarity and displays movie posters fetched from the TMDB API.

>Dataset is [HERE](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)


## Table of Contents

- [Overview](#overview)
- [Theory of Recommendation Systems](#theory-of-recommendation-systems)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model](#model)

  
## Overview

The movie recommendation system helps users discover movies similar to their favorites. By selecting a movie from the list, users receive a list of top 10 recommended movies along with their posters. This project leverages machine learning techniques to analyze the features of movies and find similarities between them. It uses the TMDB API to fetch and display movie posters, enhancing the user experience by providing visual context for the recommendations. The system is built with Streamlit, providing an interactive and user-friendly interface for users to explore movie recommendations easily.

## Theory of Recommendation Systems

### What is a Recommendation System?

A recommendation system is a subclass of information filtering systems that seek to predict the rating or preference a user would give to an item. They are widely used in various applications like movie recommendations, product recommendations, and content recommendations.

### Types of Recommendation Systems

1. **Content-Based Filtering**: This method recommends items similar to those a user liked in the past. It relies on the attributes of the items and a profile of the user's preferences.

2. **Collaborative Filtering**: This method recommends items based on the preferences of similar users. It doesn't require the attributes of the items and instead focuses on user-item interactions.

3. **Hybrid Methods**: These methods combine content-based and collaborative filtering to provide more accurate recommendations.
   

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/ankitRaj925/Movie_Recomendation_System.git
    cd Movie_Recomendation_System
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

2. Open your web browser and go to `http://localhost:8501`.

3. Select a movie from the dropdown list and click "Recommend" to get the top 10 recommended movies along with their posters.

## Dataset

The dataset used for this project contains information about movies, including their titles and IDs. It is processed and stored in `movie_data.pkl`. The dataset is used to calculate the cosine similarity between movies.

## Model

The model for recommending movies is based on cosine similarity. Cosine similarity is used to measure the similarity between movie titles. The model computes the similarity scores and suggests the top 10 similar movies based on the selected movie title.


