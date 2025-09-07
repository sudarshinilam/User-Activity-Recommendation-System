# User Activity Recommendation System

This project is a hybrid recommendation engine that suggests personalized real-world activities to users based on their interests, past interactions (ratings), and activity content (tags). It demonstrates how collaborative filtering and content-based filtering can be combined to generate accurate and relevant recommendations.

---
## 📌 Project Objective

The goal is to develop a recommendation engine that:

- Suggests **local real-world activities** tailored to individual users
- Uses a **hybrid model** combining:
  - **Collaborative Filtering** (using matrix factorization with SVD)
  - **Content-Based Filtering** (using TF-IDF and cosine similarity)
- Handles the **cold-start problem** for new users or new activities
- Can be evaluated using metrics like **Precision@k**, **Recall@k**, and **MAP** *(to be implemented)*

---
## 📂 Dataset (Synthetic)

The project uses **synthetic data** to simulate:

- **User-Activity Ratings:** How much a user liked an activity (on a scale of 1–5)
- **Activity Tags:** Keywords describing the nature of the activity (e.g., "hiking", "live music")

---

##  Techniques Used

### Collaborative Filtering (SVD)
- Builds a user-activity matrix
- Applies **Singular Value Decomposition (SVD)** to predict missing ratings
- Recommends activities based on similar users' preferences

### Content-Based Filtering
- Uses **TF-IDF vectorization** on activity tags
- Computes **cosine similarity** to find similar activities a user may enjoy

### Hybrid Recommendation
- Combines collaborative and content-based scores
- Weighted combination to balance personalization and content similarity




