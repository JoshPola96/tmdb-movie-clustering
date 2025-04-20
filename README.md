# TMDB Movie Dataset Clustering Analysis

## Project Overview
This project performs advanced clustering analysis on the TMDB (The Movie Database) 5000 movie dataset to identify patterns and groupings based on movie attributes such as budget, popularity, runtime, vote metrics, and genres. Multiple clustering algorithms (KMeans, DBSCAN, Hierarchical Clustering) are implemented and compared, with and without dimensionality reduction via PCA.

## Features
- **Data Preprocessing and Feature Engineering**
  - Creation of weighted rating system to balance vote count and average
  - Genre extraction and one-hot encoding
  - Log scaling of numeric features
  - Data standardization

- **Exploratory Data Analysis**
  - Visualization of feature relationships and correlations
  - Genre-based analysis of popularity and ratings
  - Rating classification (High, Average, Low)

- **Clustering Optimization**
  - Implementation of multiple clustering algorithms:
    - K-Means
    - DBSCAN
    - Hierarchical Clustering
  - Automatic parameter optimization via grid search
  - Dimensionality reduction using PCA with parameter tuning
  - K-Means elbow method for optimal cluster determination
  - Gap statistic implementation for cluster validation

- **Performance Evaluation**
  - Silhouette score
  - Davies-Bouldin index
  - Calinski-Harabasz index
  - Comparative analysis of clustering methods

## Technologies Used
- **Language**: Python
- **Libraries**:
  - Data manipulation: Pandas, NumPy
  - Visualization: Matplotlib, Seaborn
  - Machine Learning: Scikit-learn
  - Optimization: Joblib (parallel processing)
  - Statistics: SciPy
  - Other: Kneed (elbow detection), AST (for parsing JSON-like data)

## Dataset
The project uses the TMDB 5000 movie dataset that contains metadata for about 5,000 movies, including:
- Budget information
- Genre classification
- Popularity metrics
- Runtime details
- Vote counts and averages
- Production information

## Implementation Highlights
1. **Advanced Preprocessing Pipeline**:
   - Custom transformers for handling categorical, numerical, and multi-label data
   - Robust feature scaling and transformation

2. **Optimized Clustering Approaches**:
   - Parallel processing for efficient parameter grid search
   - Automated determination of optimal cluster numbers
   - Comparison of clustering with and without dimensionality reduction

3. **Memory-Efficient Implementation**:
   - Caching of intensive computations (e.g., gap statistic)
   - Optimized vectorization for performance

## Results
The analysis reveals distinct groupings within the movie dataset that correlate with both commercial and critical success metrics. The clusters identified provide insights into how movie attributes interact and influence overall reception.

## License
[MIT License](LICENSE)
