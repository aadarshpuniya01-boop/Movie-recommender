---

title: Movie Recommender System
emoji: "🎬"
colorFrom: indigo
colorTo: purple
sdk: streamlit
sdk_version: "1.33.0"
python_version: "3.10"
app_file: app.py
pinned: false
----

# 🎬 Movie Recommender System

A **Machine Learning-based Movie Recommendation Web App** deployed on **Hugging Face Spaces**.
This application suggests similar movies based on user selection and displays posters using the TMDB API.

---

## 🚀 Live App

👉 https://huggingface.co/spaces/Aadarshhhhhhhh/movie-recommendation

---

## 📌 Features

* 🎯 Recommends top 5 similar movies
* 🖼️ Fetches movie posters dynamically
* ⚡ Fast predictions using precomputed similarity matrix
* 🌐 Fully deployed on Hugging Face Spaces
* 🎨 Interactive UI using Streamlit

---

## 🛠️ Tech Stack

* **Frontend:** Streamlit
* **Backend:** Python
* **Machine Learning:** KNN + Cosine Similarity
* **Libraries:** Pandas, NumPy, Scikit-learn
* **API:** TMDB (for posters)

---

## 📂 Project Structure

```
.
├── app.py
├── requirements.txt
├── movie_list.pkl
├── similarity.pkl
└── README.md
```

---

## 🧠 How It Works

* Movie features (genres, keywords, cast, etc.) are processed
* A similarity matrix is created using cosine similarity
* When a user selects a movie:

  * The system finds the most similar movies
  * Returns top 5 recommendations
  * Fetches posters via TMDB API

---

## 🔑 API Configuration

The app uses **TMDB API** for posters.

* API key is stored securely in **Hugging Face Secrets**
* Accessed in code using:

```python
import os
API_KEY = os.getenv("TMDB_API_KEY")
```

---

## ⚙️ Run Locally

```bash
pip install -r requirements.txt
streamlit run app.py
```

---

## 🌍 Deployment

* Platform: **Hugging Face Spaces**
* SDK: Streamlit
* Auto deployment via `git push`
* Environment variables managed via **Secrets**

---

## 📈 Future Improvements

* 🔎 Search autocomplete
* 🎭 Genre-based filtering
* 🤖 Deep learning embeddings (BERT)
* 🎨 Netflix-style UI

---

## 👤 Author

**Adarsh**
Aspiring ML Engineer | Interested in NLP & MLOps

---

## 📄 License

MIT License


