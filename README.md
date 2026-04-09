# Assignment VIII: Student Learning Behaviour Profiling

This project aims to profile student learning behavior from the OULAD (Open University Learning Analytics Dataset) using unsupervised learning techniques. The goal is to cluster students based on their VLE interaction logs and assessment scores.

## Dataset
- **Source:** OULAD (Open University Learning Analytics Dataset)  
- Contains student interaction logs, assessment scores, and demographic information  


## Structure
- `dataset/` - OULAD raw CSV files.
- `merged.csv` - Preprocessed and combined dataset generated from the core CSVs.
- `features.csv` - Engineered features dataset used for clustering.
- `preprocessing.ipynb` - Notebook dedicated to data loading, merging, and initial preprocessing.
- `feature_engineering.ipynb` - Notebook for extracting key behavioral features.
- `clustering_and_visualization.ipynb` - Notebook for unsupervised modeling (KMeans, DBSCAN) and evaluation, PCA/T-SNE embeddings and visual feature distributions, and interpreting clusters and defining student profiles.


## Workflow

1. **Data Understanding & Preprocessing** - Loads and merges VLE interaction logs with demographic data.
2. **Feature Engineering** - Extracts key features like login frequency, activity regularity, submission delays, and early engagement proportion.
3. **Unsupervised Modelling** - Implements KMeans and DBSCAN with rigorous evaluation via Silhouette Score, Davies-Bouldin, and Calinski-Harabasz Indices.
4. **Visualization** - Shows 2D PCA/T-SNE embeddings, radar charts, and feature distributions.
5. **Ethics & Interpretations** - Translates mathematical clusters into actionable student profiles for intervention purposes.

## Technologies Used
- Python (Pandas, NumPy, Scikit-learn)  
- Matplotlib, Seaborn  
- PCA, T-SNE  
- KMeans, DBSCAN

### Feature Engineering Summary

The engineered features capture multiple dimensions of student behavior:
- Engagement (login frequency, clicks)
- Consistency (activity regularity)
- Discipline (submission delay)
- Performance (average score)

These features enable meaningful clustering of students into behavioral groups.

### Cluster Interpretation

Cluster 0: Passive Learners
- Low engagement and interaction
- Lower academic performance
- Likely to require intervention

Cluster 1: High Performers
- Very high engagement and activity
- Submit assignments early
- Achieve highest scores

Cluster 2: Moderate Learners
- Balanced engagement and performance
- Consistent but not highly active


### Key Insights

- Students with higher engagement (clicks, login frequency) perform better
- Early submission correlates with higher scores
- Low activity students form a distinct cluster of at-risk learners
- Behavioral patterns can be used to predict academic success


### Ethical & Societal Relevance

- Helps identify students needing academic support early
- Enables personalized learning strategies
- Improves student retention and success rates
- Must ensure data privacy and avoid bias in interpretation