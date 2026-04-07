# Assignment VIII: Student Learning Behaviour Profiling

This project aims to profile student learning behavior from the OULAD (Open University Learning Analytics Dataset) using unsupervised learning techniques. The goal is to cluster students based on their VLE interaction logs and assessment scores.

## Structure
- `dataset/` - OULAD raw CSV files.
- `merged.csv` - Preprocessed and combined dataset generated from the core CSVs.
- `features.csv` - Engineered features dataset used for clustering.
- `models/` - Directory for saved Joblib/Pickle models.
- `outputs/figures/` - Directory for generated plots and visualizations.
- `preprocessing.ipynb` - Notebook dedicated to data loading, merging, and initial preprocessing.
- `feature_engineering.ipynb` - Notebook for extracting key behavioral features.
- `clustering.ipynb` - Notebook for unsupervised modeling (KMeans, Hierarchical, DBSCAN, GMM) and evaluation.
- `visualization.ipynb` *(Pending)* - Notebook for PCA/UMAP embeddings and visual feature distributions.
- `ethical_analysis.ipynb` *(Pending)* - Notebook for interpreting clusters and defining student profiles.


## Workflow

1. **Data Understanding & Preprocessing** - Loads and merges VLE interaction logs with demographic data.
2. **Feature Engineering** - Extracts key features like login frequency, activity regularity, submission delays, and early engagement proportion.
3. **Unsupervised Modelling** - Implements KMeans, Hierarchical Clustering, DBSCAN and Gaussian Mixture Models with rigorous evaluation via Silhouette Score, Davies-Bouldin, and Calinski-Harabasz Indices.
4. **Visualization** - Shows 2D PCA/UMAP embeddings, radar charts, and feature distributions.
5. **Ethics & Interpretations** - Translates mathematical clusters into actionable student profiles for intervention purposes.
