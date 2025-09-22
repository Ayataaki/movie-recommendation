# movie-recommendation
A content-based movie recommendation system built with Python, Pandas, Scikit-learn, and NLTK, using cosine similarity on TMDB dataset.
# Movie Recommendation System

This project implements a **content-based movie recommendation system** using the [TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata).  
It recommends movies similar to a given one based on metadata such as **genres, keywords, cast, crew, and overview**.  

---

## Features
- Data preprocessing and cleaning (removing nulls/duplicates, parsing JSON-like fields).
- Extraction of relevant features: genres, keywords, cast, crew, overview.
- Text normalization: tokenization, lowercasing, stemming (NLTK).
- Tag creation: combining multiple metadata fields into one textual representation per movie.
- Vectorization using **CountVectorizer** (Bag of Words).
- Similarity computation using **Cosine Similarity**.
- Recommendation function: given a movie title, returns the top 5 most similar movies.

---

##  Tech Stack
- **Python 3**
- **Pandas / NumPy** (data processing)
- **Scikit-learn** (vectorization + similarity computation)
- **NLTK** (stemming)
- **Jupyter Notebook**

---

## Example
**Input:**  
```python
recommend("Batman Begins")
