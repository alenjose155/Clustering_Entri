# Clustering_Entri
# Clustering Techniques on the Iris Dataset
This project explores the application of two popular clustering algorithms—KMeans and Hierarchical Clustering—on the well-known Iris dataset. Clustering is an unsupervised learning technique used to group data based on similarity. The Iris dataset, with its numerical features and distinct natural clusters, provides an ideal case to experiment with these methods. Through this project, you'll see how KMeans efficiently creates clusters using centroid-based iterations, and how Hierarchical Clustering visually represents the cluster relationships in the form of a dendrogram.

# How KMeans Clustering Works
KMeans is a simple yet powerful clustering algorithm that aims to divide the data into a predefined number of clusters. The algorithm starts by randomly initializing cluster centroids and assigning each data point to the nearest centroid based on distance (usually Euclidean distance). Once all points are assigned, the centroids are updated by calculating the mean of all points within each cluster. This process repeats until the centroids no longer change significantly or a maximum number of iterations is reached.

# Why KMeans is a Good Fit for the Iris Dataset
The Iris dataset is entirely numerical, with each data point representing measurements of flowers across different species. KMeans handles numerical data very efficiently and is particularly effective when the data has relatively well-separated groups, as is the case with the three species in the Iris dataset. Its simplicity and speed make KMeans a natural choice for clustering tasks on smaller datasets like this one.

# How Hierarchical Clustering Works
Hierarchical Clustering takes a different approach to forming clusters. Instead of randomly initializing centroids, it builds a tree-like structure, or dendrogram, that represents the nested grouping of data points based on their similarity. In agglomerative clustering (the method used here), each data point starts as its own cluster. These clusters are then iteratively merged based on their proximity, using a linkage criterion (like Ward’s method) until all data points belong to one large cluster.

# Why Hierarchical Clustering is a Good Fit for the Iris Dataset
Hierarchical Clustering is particularly valuable when you want to understand the underlying structure of the data. For a dataset like Iris, the dendrogram provides insights into how the species are related and where the clusters naturally emerge. Since the dataset is relatively small, the computational intensity of this method is manageable, allowing us to leverage its interpretability for meaningful visualizations.

# Project Overview
This project includes the following components:

# Preprocessing: 
The Iris dataset is scaled to improve clustering performance.
# KMeans Clustering:
Clusters are created using KMeans, and their distribution is visualized.
# Hierarchical Clustering:
A dendrogram is generated to analyze cluster hierarchies, followed by a scatter plot of the clusters.
