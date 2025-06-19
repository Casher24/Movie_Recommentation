# Movie Recommendation System

## Project Overview

**Domain:** Recommender Systems  
**Use Case:** Personalized Movie Suggestions for Streaming Platforms  
**Tools Used:** Python, Surprise Library, Google Colab  

---

## Context

Online streaming platforms like **Netflix** and **Amazon Prime Video** host vast libraries of content. With so many choices, users can often feel overwhelmed. A well-designed **Recommendation System** improves user experience by surfacing personalized content, which in turn enhances **customer satisfaction** and **revenue generation** for the platform.

This project focuses on building different types of recommendation systems using a **movie ratings dataset**. The methods learned here are widely applicable to recommending books, music, e-commerce products, and more.

---

##  Objective

To build and evaluate multiple types of **Recommendation Systems** using collaborative filtering and ranking strategies:

1. ✅ **Knowledge-Based / Rank-Based Recommendation System**  
2. 🔁 **Similarity-Based Collaborative Filtering** (User-User or Item-Item)  
3. 🧩 **Matrix Factorization-Based Collaborative Filtering** (using SVD/SVD++ from Surprise Library)

---

## 📂 Dataset

We are using a simplified **MovieLens-like ratings dataset**, which contains the following fields:

| Column     | Description                          |
|------------|--------------------------------------|
| `userId`   | Unique ID for each user              |
| `movieId`  | Unique ID for each movie             |
| `rating`   | User rating of the movie (1–5)       |
| `timestamp`| Time of interaction (UNIX format)    |

The dataset simulates real user-movie interaction and serves as the input for model training and evaluation.

---

## 🛠️ Tech Stack & Tools

- **Python** – Core programming language
- **Google Colab** – Recommended environment for model building
- **Surprise Library** – For collaborative filtering algorithms
- **Pandas / NumPy** – Data preprocessing
- **Matplotlib / Seaborn** – Visualizations

> ⚠️ *Note:* The `surprise` library may have installation issues in Jupyter notebooks. It is advised to use **Google Colab** for a smoother experience.

---

##  Methodology

### 1. **Rank-Based Recommender**
- Recommends movies based on overall popularity or genre ranking
- Simple, no personalization
- Useful as a baseline

### 2. **Similarity-Based Collaborative Filtering**
- Measures similarity between users or items
- Recommends movies that similar users liked
- Uses **cosine similarity** or **Pearson correlation**

### 3. **Matrix Factorization (SVD)**
- Uses latent factors to represent users and items
- Learns hidden patterns in user preferences
- Built using `Surprise` library's SVD implementation

---

## 📈 Evaluation Metrics

- **RMSE** (Root Mean Squared Error)
- **MAE** (Mean Absolute Error)
- **Precision@K / Recall@K** (for Top-N recommendations)

---

## 📁 Project Structure

