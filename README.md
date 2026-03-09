# 🎬 Movie Recommender System

A simple yet powerful **Movie Recommendation Web App** built with **Streamlit**.  
This app suggests movies based on user input using a **KNN model with cosine similarity** trained on a Kaggle dataset.

---

## 📌 Features
- Interactive web interface powered by **Streamlit**
- Movie recommendations based on **cosine similarity** of feature vectors
- Fetches **movie posters** dynamically from **TMDB API**
- Lightweight and easy to run locally

---

## 📂 Dataset
- Source: [Kaggle Movie Dataset](https://www.kaggle.com/)  
- Preprocessed and stored as:
  - `movie_list.pkl` → contains movie metadata (titles, IDs, etc.)
  - `similarity.pkl` → precomputed similarity matrix using **KNN + cosine similarity**

---

## 🧠 Machine Learning Model
- **Algorithm:** KNN (k-nearest neighbors) with **cosine similarity**  
- **Goal:** Find the top 5 most similar movies to the selected one  
- **Steps:**
  1. Vectorize movie features (genres, overview, etc.)
  2. Compute similarity scores using cosine similarity
  3. Recommend top 5 movies with highest similarity scores

---

## 🚀 How to Run

### 1. Install Dependencies
```bash
pip install streamlit requests pickle-mixin numpy pandas scikit-learn
python -m streamlit run movierecomender.py
├── movierecomender.py      # Main Streamlit app
├── movie_list.pkl          # Pickled movie metadata
├── similarity.pkl          # Pickled similarity matrix
├── README.md               # Project documentation

