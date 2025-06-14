# 🎬 Movie Recommendation System using Machine Learning

Welcome to my **Movie Recommender System** – a machine learning-based web application built to help users discover movies tailored to their tastes. Designed using **Streamlit**, this project leverages **content-based filtering**, **collaborative filtering**, and **cosine similarity** techniques to suggest relevant movies from a dataset of popular titles.

---

## 🚀 Why Recommendation Systems?

In a world overflowing with content, recommendation systems have become essential. They help reduce decision fatigue by presenting users with personalized options based on their preferences, behavior, or interactions with similar users.

From **Netflix** to **Spotify**, these systems enhance user experience by suggesting relevant content — and that's exactly what this project does for movies!

---

## 🧠 What This System Does

🔍 This app analyzes a movie a user selects and returns **similar movies** based on:

- Movie features (genre, cast, crew, etc.)
- Other users’ preferences (if extended to collaborative filtering)
- Cosine similarity between embedded vectors

The project is designed as a practical application of data science, machine learning, and natural language processing in the entertainment domain.

---

## 🧰 Types of Recommendation Systems Used

### 1️⃣ Content-Based Filtering
- Uses attributes of items (e.g., genre, description, actors).
- Learns from a user’s history and recommends similar items.
- Example: If you liked *Inception*, you'll probably like *Interstellar*.

### 2️⃣ Collaborative Filtering (Optional/Future Scope)
- Based on past user interactions (ratings, likes).
- Learns patterns among user behaviors.
- Example: "Users who liked X also liked Y."

### 3️⃣ Hybrid Approach (Optional/Future Scope)
- Combines both methods for better accuracy.
- Balances limitations like cold-start and popularity bias.

---

## 📚 Dataset

The model uses a movie dataset containing:
- Movie titles
- Genres
- Cast & crew
- Tags and overviews

You can use datasets from [TMDB](https://www.kaggle.com/tmdb/tmdb-movie-metadata) or similar sources.

---

## 🧮 Core Concept: Cosine Similarity

Cosine similarity measures how similar two vectors are by calculating the cosine of the angle between them. It’s ideal for text-based features like movie descriptions.

```python
from sklearn.metrics.pairwise import cosine_similarity
