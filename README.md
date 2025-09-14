# User & Item-Based Recommendation System (From Scratch)

This project is a **from-scratch implementation of collaborative filtering** for building a movie recommendation system. It demonstrates both **user-based** and **item-based** approaches using **k-nearest neighbors (k-NN)** with **cosine similarity**.

---

## Overview
- Dataset format: `userid`, `movieid`, `rating`, `time` (from `data.txt`).
- Data is transformed into **user–item rating matrices** with pandas.
- Two models are implemented:
  - **User-Based Collaborative Filtering**: finds similar users and predicts ratings based on their preferences.  
  - **Item-Based Collaborative Filtering**: finds similar movies/items and predicts ratings based on related items the user has rated.
- ~20% of users and ~20% of their ratings are masked for evaluation.
- Predictions are generated using the **top-k neighbors** (default: `k=10`).
- Model accuracy is evaluated with **Root Mean Squared Error (RMSE)**.

---

## Features
- From-scratch **User-Based Collaborative Filtering**.
- From-scratch **Item-Based Collaborative Filtering**.
- Cosine similarity for similarity computation.
- k-NN prediction with weighted neighbor ratings.
- Mean-rating fallback when neighbors are uninformative.
- Pure **Python + NumPy + pandas** implementation (no external ML libraries).

---

## Example Workflow
1. Load ratings data into pandas DataFrame.
2. Create user–item and item–user pivot tables.
3. Randomly mask a subset of ratings for testing.
4. Compute cosine similarity between users (user-based) and items (item-based).
5. Predict missing ratings using k-NN with top-k neighbors.
6. Evaluate accuracy using **RMSE**.





