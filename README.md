#🎬  Ensemble-Movie-Recommendation-System
Hybrid ensemble-based movie recommendation system using CF, CBF, SVD, NCF and RNN

A hybrid ensemble-based movie recommendation system built using a combination of traditional recommendation techniques and deep learning models.  
The system integrates multiple models and fuses their predictions using a stacking-based ensemble (Linear Regression meta-learner)** to achieve higher accuracy,
robustness, and better generalization.

# 🚀 Project Motivation

Traditional recommendation systems suffer from:
- Data sparsity (users rate only a few items)
- Cold-start problem (new users/items)
- Limited expressiveness of single-model approaches

This project addresses these challenges by combining:
- Collaborative Filtering
- Content-Based Filtering
- Matrix Factorization
- Deep Learning (NCF, RNN)
- Ensemble Learning (Stacking)

---

## 🧠 Models Used

### 1. Collaborative Filtering (CF)
- User-based CF
- Item-based CF
- Similarity computed using user–item interaction matrices

### 2. Matrix Factorization (SVD)
- Latent factor modeling using Surprise library 
- Learns hidden user and movie representations

### 3. Content-Based Filtering (CBF)
- TF-IDF vectorization on movie genres
- Cosine similarity for movie-to-movie matching

### 4. Neural Collaborative Filtering (NCF)
- User and movie embeddings
- Dense neural network layers
- Captures non-linear user–item interactions

### 5. Sequential Recommendation (RNN – GRU)
- Models temporal user behavior
- Learns sequential patterns in movie consumption

### 6. Ensemble Model (Stacking)
- Combines predictions from all base models
- Linear Regression meta-learner
- Produces final predicted rating

---

##  System Architecture
<img width="1864" height="792" alt="Screenshot 2025-12-24 190808" src="https://github.com/user-attachments/assets/09396efa-9de9-4791-a500-47eca3a540c0" />


<img width="627" height="839" alt="Screenshot 2025-12-24 190820" src="https://github.com/user-attachments/assets/ef5d2581-521a-4f0b-bae7-12b25a4f76a6" />


> These diagrams illustrate:
> - Data preprocessing pipeline  
> - Individual recommendation models  
> - Ensemble fusion layer  
> - Final Top-N recommendation generation  

---



