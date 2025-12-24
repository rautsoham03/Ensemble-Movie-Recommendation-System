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
<img width="1913" height="1009" alt="Screenshot 2025-12-24 190808" src="https://github.com/user-attachments/assets/5ea26b13-0439-469d-b337-4a7b9bf743e6" />

<img width="1875" height="1016" alt="Screenshot 2025-12-24 190820" src="https://github.com/user-attachments/assets/6f7385a9-3c58-4af9-80ed-345d0595b245" />


> These diagrams illustrate:
> - Data preprocessing pipeline  
> - Individual recommendation models  
> - Ensemble fusion layer  
> - Final Top-N recommendation generation  

---



