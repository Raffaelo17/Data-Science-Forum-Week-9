<h1 align="center">DS Forum Week 9: Clustering Methods</h1>

### K-Means Clustering:

By minimizing the sum of squared distances between data points and their designated cluster centroids, K-Means clustering divides a dataset into K clusters. Each data point is assigned to the cluster with the nearest mean.</br></br>
scalable and effective for big datasets.
functions best in spherically shaped, uniformly sized clusters.</br>

Sensitive to the centroids' original selection. Assumes equal sizing and sphericity of clusters, which may not be the case for all datasets.</br></br>


### Hierarchical Clustering:

By repeatedly joining or dividing clusters, hierarchical clustering creates a tree of clusters. A dendrogram, which is a hierarchy of clusters, is the end product. The dendrogram can be clipped at a specific height to determine the number of clusters.<br><br>
Advantages: Shows the data's hierarchical structure.
There's no need to predetermine the number of clusters.</br>
Cons: Costlier to compute, particularly for big datasets.
Subjective interpretation is possible.<br><br>

### DBSCAN (Density-Based Spatial Clustering of Applications with Noise):

DBSCAN is a density-based clustering technique that classifies outliers as noise and clusters together data points that are sufficiently close to one another and have enough neighbors. The number of clusters need not be specified.</br>
Advantages: Capable of finding groups of any shape.
robust against anomalies and noise.</br>
Cons: Dependent on the hyperparameters and distance metric selected.
High-dimensional spaces may result in a decline in performance.</br></br>

### Gaussian Mixture Model (GMM):

A combination of Gaussian distributions is represented by the probabilistic model known as the GMM. It use the Expectation-Maximization (EM) algorithm to estimate the parameters and makes the assumption that the data points are produced from a combination of multiple Gaussian distributions.</br>
Advantages: Capable of simulating clusters of various sizes and shapes.
gives soft assignments, or the likelihood that every point belongs to every cluster.</br>
Cons: Dependent on the initial parameter selection.
more computationally costly than K-Means.</br></br>

<h2 align="center">Results and Assessment</h2>
The evaluation metrics for the various clustering techniques used on the dataset are shown in the following table:

</br></br>
