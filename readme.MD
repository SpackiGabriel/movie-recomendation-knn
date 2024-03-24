# Movie Recommendation System

This project aims to create a movie recommendation system based on user ratings.

## Description

The project utilizes movie ratings data and movie information to build a simple recommendation system, using the k-nearest neighbors (KNN) algorithm.

## Functionality

1. **Data Preparation:**
   - Data is loaded from CSV files using the Pandas library.
   - The data is cleaned and prepared for analysis, including selecting relevant features and handling missing data.

2. **Modeling:**
   - Data is organized and transformed to create a sparse matrix representing user ratings for movies.
   - The k-nearest neighbors model is trained using the sparse matrix.

3. **Recommendations:**
   - A `getSuggestions()` function is defined to provide movie recommendations based on an input movie.

## Requirements

- Python 3
- Pandas
- SciPy
- scikit-learn

## How to Use

1. Make sure you have the requirements installed.
2. Run the provided script in your Python environment.
3. Use the `getSuggestions(movie_name)` function to receive movie recommendations based on the input movie name.

Example Usage:

```python
from random import choice

suggestions = getSuggestions('Toy Story')
print(choice(suggestions))
