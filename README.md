# Movie Recommender System 🎬

A content-based movie recommender system that suggests the top 5 most similar movies based on various factors like actors, genres, director, and movie overview. This project uses data from The Movie Database (TMDB) and applies natural language processing techniques to make meaningful recommendations.

## Features 🔥

- **Data Preprocessing**: The dataset is cleaned and preprocessed to ensure better quality recommendations. This includes:
  - Lowercasing text for uniformity.
  - Merging cast and crew names into single-word entities (e.g., `TomHanks`).
  - Combining important metadata such as actors, genres, director, and movie overview into one column for vectorization.
  
- **Vectorization**: We use `CountVectorizer` to convert the metadata into a vectorized form that captures the frequency of words.

- **Cosine Similarity**: The similarity between movies is calculated using cosine similarity, which allows us to compare the vectorized metadata of each movie and find the most similar ones.

- **Top 5 Recommendations**: For any given input movie, the system recommends the top 5 most similar movies.

  ![image](https://github.com/user-attachments/assets/fea4c020-2640-491b-ad0b-d583db13609b)


### Libraries Used

- Python 3.x
- Required Python Libraries:
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `streamlit`
