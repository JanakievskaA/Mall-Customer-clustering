# Customer Segmentation with Clustering

This project performs customer segmentation using clustering techniques on a dataset of mall customers. The goal is to group customers based on their annual income and spending score, enabling businesses to better understand their customer base and develop targeted marketing strategies.

## Project Overview

In this project, we apply two popular clustering algorithms:
1. **K-Means Clustering**
2. **Hierarchical Clustering (Agglomerative)**

We evaluate the performance of both algorithms using various metrics, such as the **Silhouette Score** and **Davies-Bouldin Index**. Visualizations, such as Elbow Method and Dendrogram, are also included to determine the optimal number of clusters and to understand the clustering structure.

## Dataset

The dataset used in this project contains the following columns:
- **CustomerID**: Unique identifier for each customer
- **Gender**: Gender of the customer (Male/Female)
- **Age**: Age of the customer
- **Annual Income (k$)**: Annual income of the customer in thousands of dollars
- **Spending Score (1-100)**: A score assigned to the customer based on spending behavior

## Steps Involved

### 1. Data Preprocessing
- Loading and inspecting the dataset
- Handling any missing values (if applicable)
- Selecting features for clustering (Annual Income and Spending Score)
- Standardizing the features using `StandardScaler` to normalize the data

### 2. Clustering
- **K-Means Clustering**: 
  - Used the Elbow method to determine the optimal number of clusters.
  - Applied K-Means clustering with 5 clusters.

- **Hierarchical Clustering**:
  - Used Agglomerative Clustering to group customers into 5 clusters.
  - Generated a dendrogram to visualize the hierarchical structure of clusters.

### 3. Evaluation
- **Silhouette Score**: Measures how similar each point is to its own cluster compared to other clusters.
- **Davies-Bouldin Index**: Evaluates the average similarity ratio of each cluster with the one that is most similar to it.

### 4. Visualization
- Visualized the clusters using scatter plots with different color palettes for K-Means and Hierarchical Clustering.
- Generated an Elbow plot to identify the optimal number of clusters for K-Means.
- Created a dendrogram for Hierarchical Clustering to visualize the clustering process.

## Key Metrics

- **Silhouette Score**:
  - K-Means: 0.55
  - Hierarchical Clustering: 0.55

- **Davies-Bouldin Index**:
  - K-Means: 0.57
  - Hierarchical Clustering: 0.58

## Conclusion
- After evaluating both methods using the Silhouette Score and Davies-Bouldin Index, both models performed similarly, with K-Means slightly outperforming Hierarchical Clustering in terms of both metrics.
