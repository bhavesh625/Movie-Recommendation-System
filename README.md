# Movie-Recommendation-System
Project Overview

This project focuses on building a Movie Recommendation System that recommends movies based on content similarity. By utilizing Count Vectorizer to extract features from movie descriptions (plot, genres, cast, etc.) and **Cosine Similarity **to measure the similarity between movies, the system suggests movies that are most similar to a given movie.

Features

Preprocessing of movie metadata (such as plot, cast, genre)
Feature extraction using Count Vectorizer (Bag of Words)
Similarity calculation using Cosine Similarity
Movie recommendation based on content similarity
Dataset

The dataset used contains information about movies, including: Id Title (The title of the movie) Genres (The genre(s) of the movie) Overview (A brief description of the movie plot) Popularity Release-Date Vote-Average Vote-Count

Requirements

The following libraries are required to run the project:

Python 3.x
numpy (for numerical computations)
pandas (for handling data frames)
scikit-learn (for count vectorization and similarity computation)
nltk (for natural language processing tasks)
Project Structure:

Preprocessing

Data Cleaning: (i) Remove missing or invalid data. (ii) Standardize text data (lowercasing, removing special characters, etc.)

Feature Engineering: (i) Combine relevant features like genres, overview, keywords, and cast into a single metadata column for analysis. (ii) Convert text-based features into numerical vectors using Count Vectorizer (Bag of Words model).

Feature Extraction using Count Vectorizer

Count Vectorizer converts the textual data into a matrix of token counts, allowing the model to analyze the frequency of words in movie descriptions.

This vectorized data is used to compare movies by measuring the Cosine Similarity between their feature vectors.

Cosine Similarity is a metric used to measure how similar two movies are based on their vectorized features.

How the Movie Recommendation Works

Input: The user provides the title of a movie.
Vectorization: The system vectorizes the movie metadata (such as the overview, genre, cast) using Count Vectorizer.
Similarity Calculation: Using Cosine Similarity, the system compares the input movie with all other movies in the dataset.
Recommendation: The system sorts the movies by similarity and recommends the top n most similar movies.
Conclusion

The system will recommend the top n movies based on their similarity to the input movie.
