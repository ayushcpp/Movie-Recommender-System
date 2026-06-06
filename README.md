# 🎬 Movie Recommender System

A content-based Movie Recommender System built using Python, Pandas, Scikit-Learn, and Streamlit.

This project recommends movies similar to the movie selected by the user using cosine similarity.

---

## Features

- Recommend similar movies
- Content-based filtering
- Cosine similarity algorithm
- Streamlit web interface
- Uses TMDB movie dataset

---

## Tech Stack

- Python
- Pandas
- NumPy
- Scikit-Learn
- NLTK
- Streamlit

---

## Dataset Used

- `tmdb_5000_movies.csv`
- `tmdb_5000_credits.csv`

---

## Project Structure

```text
├── Data
│   ├── tmdb_5000_movies.csv
│   └── tmdb_5000_credits.csv
├── movie-recomender-system.ipynb
├── app.py
├── movie_dict.pkl
├── similarity.pkl
├── requirements.txt
└── README.md
```

---

## How Recommendation Works

1. Merge movie and credits dataset
2. Extract important features:
   - Genres
   - Keywords
   - Cast
   - Crew
   - Overview
3. Perform preprocessing and stemming
4. Create tags for every movie
5. Convert text into vectors using CountVectorizer
6. Calculate cosine similarity
7. Recommend the most similar movies

---

## Installation

Clone the repository:

```bash
git clone <your-repository-url>
cd Movie-Recommender-System
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the Streamlit app:

```bash
streamlit run app.py
```

---

## Important

Before running `app.py`, run the notebook first:

```bash
movie-recomender-system.ipynb
```

Running the notebook will generate:

- `movie_dict.pkl`
- `similarity.pkl`

These files are required for the Streamlit application to work properly.

---

## TMDB API Issue

Originally, this project was planned to use the TMDB API.

With API integration:

- Movie posters would appear automatically
- Real-time movie information could be fetched
- Better movie details would be available

However, during development, the TMDB website/API was not accessible properly, so the API key could not be obtained and configured.

Because of this, the current project uses only the downloaded TMDB dataset and does not display movie posters.

If TMDB API access becomes available later, this project can easily be upgraded into a fully API-based movie recommender system.

---

## Future Improvements

- Add TMDB API integration
- Display movie posters
- Add ratings and release dates
- Improve recommendation quality
- Deploy online

---

## Author

Ayush Gairola