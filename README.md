# Anomaly-detection-isolationforest-dbscan
Anomaly detection and clustering project using Isolation Forest and DBSCAN to detect unusual customer behavior from TripAdvisor review data.

## Project Overview

**Objective:**  
Identify anomalous users and group similar users to understand behavioral patterns and detect potential outliers in the TripAdvisor review data.

**Dataset:**  
The dataset (`tripadvisor_reviews.csv`) consists of 980 users with their average ratings in four categories:
- `avg_museum_rating`
- `avg_park_rating`
- `avg_restaurant_rating`
- `avg_nightlife_rating`

## Project Steps

1. **Data Loading and Exploration**
   - Loaded TripAdvisor review data
   - Checked for missing values and verified data consistency

2. **Preprocessing**
   - Feature scaling using `StandardScaler`
   - Optional dimensionality reduction using `PCA` for visualization

3. **Anomaly Detection**
   - Applied `IsolationForest` with contamination set to estimate proportion of anomalies
   - Visualized anomaly scores and identified unusual rating profiles

4. **Clustering**
   - Implemented `DBSCAN` to identify groups of similar users
   - Tuned `eps` and `min_samples` to maximize silhouette score
   - Visualized clusters and noise points in PCA-reduced space
