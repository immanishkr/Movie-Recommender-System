:

🎬 Movie Recommender System using TMDB Dataset
📘 Project Overview

This project is a content-based movie recommender system built using the TMDB (The Movie Database) dataset.
It suggests movies similar to the one selected by the user based on feature similarity (like genre, keywords, and overview).

The system is deployed using Streamlit, allowing users to interact with the model and view movie posters fetched from the TMDB API.

🧠 Objective

To build an intelligent system that:

Recommends movies similar to the one selected by the user.

Enhances the movie discovery experience using machine learning and data science.

Integrates live poster images via TMDB API for a user-friendly experience.

🛠️ Tech Stack

Languages: Python
Libraries: Pandas, NumPy, Scikit-learn, Pickle, Streamlit, Requests
API: TMDB API (for movie metadata and posters)
Dataset: TMDB 5000 Movie Dataset (includes tmdb_5000_movies.csv and tmdb_5000_credits.csv)

📂 Project Structure
├── app.py                         # Streamlit app for movie recommendation
├── notebook86c26b4f17.ipynb       # Jupyter Notebook for data preprocessing and model creation
├── model/
│   ├── movie_list.pkl             # Pickled dataframe of movie metadata
│   └── similarity.pkl             # Pickled cosine similarity matrix
├── dataset/
│   ├── tmdb_5000_movies.csv
│   └── tmdb_5000_credits.csv
└── README.md                      # Project documentation

⚙️ Working of the Model

Data Preprocessing:

Merged movie and credit datasets.

Extracted relevant features: genres, keywords, overview, cast, crew.

Applied text cleaning and transformation (lowercasing, stemming, removing stopwords).

Feature Engineering:

Combined text-based features into a single column.

Converted text to vectors using CountVectorizer.

Calculated cosine similarity between movies to measure closeness.


Saved movie metadata and similarity matrix using Pickle.

Deployed via Streamlit for real-time movie recommendations.
