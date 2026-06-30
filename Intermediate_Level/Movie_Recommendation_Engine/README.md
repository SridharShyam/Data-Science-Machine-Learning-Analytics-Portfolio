# Hybrid Movie Recommendation Engine

## Project Overview

With thousands of movies available on modern streaming platforms, users often spend more time searching for content than actually watching it. This project develops a Hybrid Movie Recommendation System using the MovieLens dataset to suggest movies that align with a user's interests, thereby improving engagement and customer satisfaction.

The solution combines Content-Based Filtering and Collaborative Filtering (Matrix Factorization) to generate highly personalized movie recommendations. It follows an end-to-end machine learning workflow, including data exploration, feature engineering, model development, evaluation, and recommendation generation.

## Models Evaluated

Several recommendation approaches are developed and combined in this project:
- Content-Based Filtering (using TF-IDF and Cosine Similarity)
- Collaborative Filtering (Matrix Factorization using Singular Value Decomposition/SVD)
- Hybrid Recommendation System (combining Content-Based and Collaborative Filtering)

## Libraries Used

- `pandas` and `numpy` for data manipulation
- `matplotlib` and `seaborn` for data visualization
- `scikit-learn` for machine learning algorithms and TF-IDF vectorization
- `scikit-surprise` for collaborative filtering algorithms (SVD)

## Workflow

1. **Load Data**: The `movies.csv`, `ratings.csv`, and `tags.csv` datasets from MovieLens are loaded and inspected.
2. **Exploratory Data Analysis (EDA)**: Understanding dataset sizes, sparsity, and user-movie interaction patterns.
3. **Content-Based Filtering**: Building a recommendation model based on movie genres and user tags.
4. **Collaborative Filtering**: Implementing Matrix Factorization to recommend movies based on historical user rating patterns.
5. **Hybrid System**: Combining both approaches to mitigate their individual limitations and improve recommendations.
6. **Model Evaluation**: Assessing model performance using Root Mean Square Error (RMSE) and other recommendation-specific evaluation metrics.

## How to Run

Open the `Movie_Recommendation_Engine.ipynb` Jupyter Notebook and run the cells sequentially. Make sure you have the required libraries installed and the dataset files (`movies.csv`, `ratings.csv`, `tags.csv`) in the appropriate directory as referenced in the notebook.

## Credits

Dataset provided by [GroupLens Research (MovieLens)](https://grouplens.org/datasets/movielens/).
