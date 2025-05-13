# 🎬 Content-Based Movie Recommendation System

This project recommends movies based on metadata (genres, cast, crew, keywords, overview) using a **content-based filtering approach** and **cosine similarity**.

##  Features

- Recommends movies similar to a given title
- Uses NLP to preprocess movie metadata
- Implements cosine similarity for finding related movies
- Cleaned and engineered features from TMDB dataset
- Simple Python implementation, ready for deployment

##  How it Works

1. Load and merge movie and credits datasets
2. Extract features: genres, keywords, cast (top 3), director, overview
3. Clean and preprocess text (lowercase, stemming, stop word removal)
4. Create a combined feature (`tags`) column
5. Convert text to vectors using `CountVectorizer`
6. Compute cosine similarity between movie vectors
7. Recommend top N similar movies to a given input

##  Dataset

- `tmdb_5000_movies.csv`
- `tmdb_5000_credits.csv`

Source: [The Movies Dataset - Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

##  Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/Kruthi15/content-movie-recommender.git
cd content-movie-recommender
