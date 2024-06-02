# Movie Recommender System using Cosine Similarity

## Introduction
This project is a content-based movie recommender system that suggests movies to users based on the similarity of movie content. The system uses cosine similarity to measure the similarity between movies based on their genres, keywords, and other relevant features.

## Features
- Recommend movies based on content similarity.
- Utilize cosine similarity to find similar movies.
- Provide recommendations based on movie genres, keywords, and more.

## Dataset
The dataset used in this project contains information about movies, including:
- Movie titles
- Genres
- Keywords
- Other relevant features
- link - https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata

## Installation
To run this project, you need to have Python and pip installed. Follow the steps below to set up the project:

Clone the repository:
   ```bash
   git clone https://github.com/Aditya-Ranjan1234/Movie_Recommendation.git
   ```

## Usage
   - Enter movie name in recommend functions.

## Methodology
The recommender system uses a content-based filtering approach to suggest movies. The key steps are as follows:

1. **Data Preprocessing**: Clean and preprocess the movie data, including handling missing values and transforming data into the required format.

2. **Feature Extraction**: Extract relevant features such as genres and keywords from the dataset.

3. **Vectorization**: Convert text features into vectors using techniques such as TF-IDF.

4. **Similarity Calculation**: Compute the cosine similarity between movie vectors to measure their similarity.

5. **Recommendation**: Recommend movies based on their similarity to the target movie.

## Example Code Snippet

Here's a basic example of how the cosine similarity is calculated in the project:

```python
from sklearn.metrics.pairwise import cosine_similarity
from sklearn.feature_extraction.text import TfidfVectorizer

# Sample data
movies = ["Action Adventure", "Comedy Drama", "Sci-Fi Thriller"]

# Vectorize the movie genres
vectorizer = TfidfVectorizer()
tfidf_matrix = vectorizer.fit_transform(movies)

# Calculate cosine similarity
cosine_sim = cosine_similarity(tfidf_matrix, tfidf_matrix)

print(cosine_sim)
```
## Credits

This code was originally created by CampusX (@campusx-official).
Code had been further modified.
