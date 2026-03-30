# fashion-recommendation-system

https://sara-iqbal.github.io/fashion-recommendation-system/

### Hybrid Collaborative + Content-Based Filtering

A sophisticated recommendation system designed for fashion e-commerce, utilizing a hybrid approach to overcome the "Cold Start" problem and provide personalized shopping experiences.

##  Overview
This project implements a multi-tier recommendation strategy to suggest clothing and accessories based on both item attributes and user behavior patterns.

### Key Features
* **Synthetic Data Generation**: Simulates 500 items across 7 categories (Tops, Shoes, etc.) and 2,000 unique user profiles.
* **Content-Based Filtering**: Uses **Cosine Similarity** on one-hot encoded item features (style, color, season, price).
* **Collaborative Filtering**: Implements **Matrix Factorization** via **Truncated SVD** to identify latent patterns in user-item interactions.
* **Hybrid Scoring**: Blends content and collaborative scores with a tunable alpha ($\alpha$) parameter to optimize for both accuracy and variety.
* **Automated Evaluation**: Tracks **Recall@20** and **Precision@10**, demonstrating the performance gain of the hybrid model over standalone methods.

##  Results
The engine generates a visual analytics dashboard (`fashion_rec_results.png`) and a structured JSON export (`fashion_rec_data.json`) summarizing:
* Item distribution by category and style.
* Rating distributions and SVD explained variance.
* Precision comparison between Hybrid and Collaborative-only models.

##  Installation
1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/fashion-recommendation-system.git](https://github.com/yourusername/fashion-recommendation-system.git)
