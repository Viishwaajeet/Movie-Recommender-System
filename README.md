# Movie Recommender System

This repository contains a simple content-based movie recommendation system built with Python and Streamlit. It leverages movie metadata to calculate similarity scores between films and then provides movie suggestions based on a selected title.

## Overview

In a world where countless movies are released and available on various platforms, it can be challenging to decide what to watch next. This Movie Recommender System helps users discover new films similar to the ones they already love. By analyzing movie attributes and computing similarity scores, it can generate personalized suggestions with a single click.

A live demo of the app is available at:  
**Movie Recommender App**

## Features

- **Content-Based Recommendations:** Suggests movies based on metadata (e.g., titles, overviews, or other attributes).
- **Interactive Interface:** Built with Streamlit for an easy-to-use web-based experience.
- **Fast and Efficient:** Precomputed similarity scores (stored in `similarity.pkl`) ensure quick responses.
- **Easy to Extend:** Can be modified to include additional features (e.g., genres, cast, crew, keywords).

## How It Works

- **Data Loading:** The system loads a preprocessed dataset of movies (stored in `movies.pkl`).
- **Similarity Matrix:** A precomputed similarity matrix (`similarity.pkl`) uses techniques like cosine similarity on relevant features (e.g., plot overviews, keywords, genres, or cast).
- **User Input:** The user selects a movie from a dropdown list in the Streamlit app.
- **Recommendation:** The system finds the top 5 most similar movies by looking up the corresponding row in the similarity matrix and returns them to the user.

## Technologies Used

- **Python:** Core programming language for data processing and model building.
- **Pandas:** Used for handling and manipulating the movie dataset.
- **Streamlit:** Provides a quick and interactive web interface.
- **Pickle:** Used for saving and loading the precomputed data and similarity matrix.
- **(Optional) scikit-learn / NLP libraries:** Could be used in feature extraction or more advanced similarity computations.
