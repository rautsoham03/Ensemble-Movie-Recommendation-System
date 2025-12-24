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
<img width="1200" height="300" alt="Screenshot 2025-12-24 190808" src="https://github.com/user-attachments/assets/09396efa-9de9-4791-a500-47eca3a540c0" />


<img width="327" height="539" alt="Screenshot 2025-12-24 190820" src="https://github.com/user-attachments/assets/ef5d2581-521a-4f0b-bae7-12b25a4f76a6" />


> These diagrams illustrate:
> - Data preprocessing pipeline  
> - Individual recommendation models  
> - Ensemble fusion layer  
> - Final Top-N recommendation generation  

---

---

## 📊 Dataset

This project uses the **MovieLens 100K** dataset.

Included files:
- `movielens100k.csv` – cleaned dataset
- `train_data.csv` – training split
- `test_data.csv` – testing split

Original dataset source:
https://grouplens.org/datasets/movielens/100k/

---


### How to Run the Project

### 1. Clone the Repository

git clone https://github.com/rautsoham03/Hybrid-Deep-Learning-Based-Personalized-Recommendation-System

### 2. Install Dependencies
pip install -r requirements.txt

### 3. Data Preprocessing
python src/data_processing/movielens100k.py

### 4. Train Individual Models
python src/models/cf_model_fixed.py
python src/models/content_based_filtering.py
python src/models/hypertuned_models.py
python src/models/fix_ncf_predictions.py
python src/models/rnn_sequential.py

### 5. Ensemble Prediction

The ensemble combines outputs from all base models using
Linear Regression stacking to generate final predicted ratings
and Top-N movie recommendations. 

📈 Evaluation Metrics

RMSE
MAE
Precision
Recall
F1-Score

