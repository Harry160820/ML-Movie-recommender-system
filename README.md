# ML-Movie-recommender-system

This project implements a Content-Based Movie Recommendation System using the TMDB 5000 movies dataset. The model recommends movies based on the similarity of features such as genres, keywords, cast, crew, and the movie overview.

## Project Overview
In this project, I created a movie recommendation engine using Natural Language Processing (NLP) techniques and cosine similarity. The main goal is to recommend movies that are similar to the one a user likes based on the content of the movie.

## Key Features:
-> **Data Cleaning**: Merged two datasets (movies and credits) and handled missing or duplicate data.

-> **Feature Engineering:** Extracted and transformed key movie features such as genres, keywords, cast, crew, and the movie overview.

-> **Text Preprocessing:**

1) Converted the textual data (genres, keywords, etc.) to a simplified format using stemming.
2) Removed unnecessary spaces and standardized the text for comparison.

-> **Vectorization:** Utilized CountVectorizer to convert the processed text into a matrix of token counts.

-> **Cosine Similarity:** Computed the cosine similarity between movie vectors to find similar movies.

-> **Recommendation System:** Built a function that recommends the top 5 most similar movies based on the input movie's content.

# Dataset:
1) **tmdb_5000_movies.csv:** Contains information about movies like title, overview, genres, and keywords.
2) **tmdb_5000_credits.csv:** Contains details about the cast and crew of the movies.

# Libraries Used

-> **pandas** for data manipulation
-> **numpy** for numerical operations
-> **nltk** for text preprocessing (stemming)
-> **sklearn** for vectorization and cosine similarity calculation

# How It Works
1) **Data Merging:** The movies and credits datasets are merged on the movie title.
2) **Feature Extraction:** We extract relevant columns such as genres, keywords, cast, crew, and overview, and convert them into a standardized format.
3) **Text Preprocessing:** The text data is cleaned, tokenized, and stemmed for better comparison
4) **Vectorization:** The tags (combined feature) are converted into vectors using CountVectorizer.
5) **Similarity Calculation:** Cosine similarity is calculated to measure the similarity between movies based on the feature vectors.
6) **Recommendations:** Given a movie title, the system returns the top 5 most similar movies.

# Example
For the movie **"Batman Begins"**, the top 5 recommended movies are:

The Dark Knight
The Dark Knight Rises
Batman
Batman & Robin
Batman


