README for Lab 3

# Lab 3: Clustering Using K-Means and K-Medoids

## Course
Advanced Big Data and Data Mining  
Spring 2026  

## Student
Mounisha Yarava  

## Overview
This lab explores unsupervised learning techniques:
- K-Means Clustering
- K-Medoids Clustering

The objective is to group data points into clusters and evaluate clustering quality using metrics.

## Dataset
- Source: Scikit-learn
- Name: Wine Dataset
- Samples: 178
- Features: 13 numerical attributes

## Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Scikit-learn-extra

## Implementation Details

### 1. Data Preprocessing
- Standardized dataset using Z-score normalization


### 2. K-Means Clustering
- Number of clusters (k) = 3

Evaluation Metrics:
- Silhouette Score
- Adjusted Rand Index (ARI)

Observations:
- Well-separated clusters
- Higher silhouette score
- Strong alignment with actual labels

### 3. K-Medoids Clustering
- Number of clusters (k) = 3

Observations:
- More robust to outliers
- Slightly lower performance than K-Means
- Uses actual data points as cluster centers

## Results

| Algorithm   | Silhouette Score | ARI Score |
|------------|----------------|----------|
| K-Means    | Higher         | Higher   |
| K-Medoids  | Slightly Lower | Moderate |

## Visualization
- Scatter plots comparing:
  - K-Means clusters
  - K-Medoids clusters

## Key Differences

| Feature          | K-Means        | K-Medoids      |
|-----------------|---------------|----------------|
| Cluster Center  | Centroid       | Actual Data Point |
| Speed           | Faster         | Slower         |
| Outlier Handling| Less Robust    | More Robust    |


## Challenges
- Importance of feature scaling
- Understanding evaluation metrics (Silhouette & ARI)
- Ensuring fair comparison between models


## Conclusion
K-Means performed better for this dataset with clearer clusters.  
K-Medoids is useful when robustness to noise and interpretability are required.

## How to Run
pip install numpy pandas matplotlib scikit-learn scikit-learn-extra
