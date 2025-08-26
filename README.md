# 🎬 Movie Recommendation System

A **content-based Movie Recommendation System** built using  
**Python, Pandas, Scikit-learn, and Streamlit**.  

It recommends **top 5 similar movies** for a given input movie and displays posters using the **TMDB API**.  

---

## 🚀 Features
- Recommends movies based on content similarity.
- Displays **movie posters + titles**.
- Uses **CountVectorizer + Cosine Similarity** for recommendations.
- Interactive UI built with **Streamlit**.
- Automatically generates `movies1.pkl` and `similarity.pkl` from CSVs if not present.

---

## 📊 Dataset
The project uses the following CSV files (already included in this repo):
- `tmdb_5000_movies.csv`
- `tmdb_5000_credits.csv`

---

## 🔧 How It Works
1. Reads the TMDB dataset (`tmdb_5000_movies.csv`, `tmdb_5000_credits.csv`).
2. Extracts features like **genres, keywords, cast, crew, overview**.
3. Combines them into a single text field called **tags**.
4. Uses **CountVectorizer** to convert tags into vectors.
5. Computes **cosine similarity** between movies.
6. Returns **top 5 most similar movies** with posters from TMDB API.

1. Clone the repo:
   ```bash
   git clone https://github.com/rahul941174/Movie_Recommendation_System.git
   cd Movie_Recommendation_System
