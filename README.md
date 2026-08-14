# A-Comparative-Study-of-Hybrid-KNN-Autoencoders-and-Deep-Metric-Learning-with-Triplet-Loss
# Women's Fashion Recommendation System

A content-based product recommendation system developed using a dataset
of 50,000 women's fashion products.

## Objective

The goal is to recommend similar products when no user-product interaction
data is available.

## Approaches

### 1. Hybrid KNN
Combines:

- Content similarity
- Price similarity

### 2. Autoencoder
Learns a latent representation of products through multi-task reconstruction.

### 3. Neural Embedding with Triplet Loss
Learns a product embedding space where:

- similar products are close together
- different products are separated

## Evaluation

The models are evaluated using:

- Category Match@5
- Subcategory Match@5
- Mean Relative Price Gap

## Results

| Model | Category Match@5 | Subcategory Match@5 | Price Gap |
|---|---:|---:|---:|
| Hybrid KNN | 0.998 | 0.928 | 0.121 |
| Autoencoder | 0.997 | 0.993 | 0.396 |
| Neural Embedding | 0.993 | 0.996 | 0.155 |

The Hybrid KNN achieves the best price proximity, while the Neural
Embedding model obtains the best subcategory coherence.

## Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
