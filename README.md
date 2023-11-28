<h1 align="center">DS Forum Week 9: Clustering Methods</h1>

### K-Means Clustering:

By minimizing the sum of squared distances between data points and their designated cluster centroids, K-Means clustering divides a dataset into K clusters. Each data point is assigned to the cluster with the nearest mean.</br></br>
scalable and effective for big datasets.
functions best in spherically shaped, uniformly sized clusters.</br>

Sensitive to the centroids' original selection. Assumes equal sizing and sphericity of clusters, which may not be the case for all datasets.</br></br>

Results:
Silhouette Score: 0.1264364314825275
Davies-Bouldin Index: 2.445935417058955
Rand Score: 0.2216930048692321
Calinski and Harabasz Score: 221.11727444263212
### Means Shift Clustering:

Seeks to identify "blobs" within a sample density that is smooth. This approach, which is based on centroid selection, updates potential centroids to be the average of the points in a certain area.<br><br>
Advantages: Shows the data's hierarchical structure.
There's no need to predetermine the number of clusters.</br>
Cons: Costlier to compute, particularly for big datasets.
Subjective interpretation is possible.<br><br>

Results:

### Agglomerative Clustering:

The most popular kind of hierarchical clustering, which organizes things according to how similar they are. Another name for it is Agglomerative Nesting, or AGNES. Every object is first viewed by the algorithm as a singleton cluster. Subsequently, clusters are combined in pairs until all clusters are combined into a single large cluster that contains all of the objects. The ultimate product is a dendrogram, which is an object representation based on a tree.</br>
Advantages: Capable of finding groups of any shape.
robust against anomalies and noise.</br>
Cons: Dependent on the hyperparameters and distance metric selected.
High-dimensional spaces may result in a decline in performance.</br></br>

Results:
Silhouette Score: 0.11077086341414898
Davies-Bouldin Index: 2.7497403469949773
Rand Score: 0.2981967298269896
Calinski and Harabasz Score: 193.63464529209537

### Spectral Clustering:

Use the data's similarity matrix's spectrum, or eigenvalues, to reduce the number of dimensions before clustering the data into smaller groups. A quantitative evaluation of the relative similarity between every pair of points in the dataset makes up the similarity matrix, which is supplied as an input.</br>
Advantages: Capable of simulating clusters of various sizes and shapes.
gives soft assignments, or the likelihood that every point belongs to every cluster.</br>
Cons: Dependent on the initial parameter selection.
more computationally costly than K-Means.</br></br>

<h2 align="center">Results and Assessment</h2>
The evaluation metrics for the various clustering techniques used on the dataset are shown in the following table:

</br></br>

Results:
Silhouette Score: 0.012947828868357035
Davies-Bouldin Index: 0.8701680179286883
Rand Score: 5.189135899521916e-07
Calinski and Harabasz Score: 1.3133090439623518
