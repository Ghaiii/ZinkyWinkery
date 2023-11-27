# Unsupervised Machine Learning Evaluation Code: Wine Dataset

- KMeans:

Description: KMeans is a centroid-based clustering algorithm. It partitions the dataset into 'k' clusters by assigning each data point to the cluster whose centroid is closest.
Pros: Simple and computationally efficient. Works well when clusters are spherical and have similar sizes.
Cons: Sensitive to initial centroid placement. May not perform well on non-spherical or unevenly sized clusters.

- Hierarchical Clustering:

Description: Hierarchical clustering builds a hierarchy of clusters. It can be agglomerative (start with individual data points and merge them) or divisive (start with one cluster and split it).
Pros: No need to specify the number of clusters beforehand. Captures hierarchical relationships in the data.
Cons: Computationally intensive for large datasets.

- DBSCAN (Density-Based Spatial Clustering of Applications with Noise):

Description: DBSCAN is a density-based clustering algorithm. It groups together data points that are close to each other and have a sufficient number of neighbors.
Pros: Can discover clusters of arbitrary shapes. Robust to noise and outliers.
Cons: Sensitive to hyperparameter settings. Requires careful tuning of parameters like epsilon and minimum points.

- Gaussian Mixture Model (GMM):

Description: GMM assumes that the data is generated from a mixture of several Gaussian distributions. It represents the data as a combination of these distributions.
Pros: Soft clustering (assigns probabilities to data points belonging to each cluster). Can handle clusters with different shapes and sizes.
Cons: Sensitive to initialization. May converge to local optima.


These algorithms serve different purposes and are suited for different types of data and clustering scenarios. The choice of algorithm depends on factors such as the shape of the clusters, dataset size, and the desired outcome of the clustering analysis. Evaluating their performance using metrics like Jaccard Score, Rand Score, Calinski and Harabasz Score, Silhouette Score, and Davies Bouldin Index can help determine which algorithm performs best for a particular dataset.
