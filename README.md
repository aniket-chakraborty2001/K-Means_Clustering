# K-Means_Clustering
This project covers a clustering algorithm based on a Kc_Housing data set

## About Project:
This project covers a unsupervised learning algorithm clustering. The algorithm that is used here is called K-Means clustering. To do this, we need to satisfy two criterias. They are - 
* We consider only numeric data. (For categorical data, we use dummy encoding)
* We need to standardize the numerical column (For this we use Z-score conversion). This is also called scaling
Then we use KMeans module of sklearn library and make clustering models using a specified number of clusters. We get the labels and centers of the models.

To check the optimal number of clusters we plot the elbow plot and observe that some clusters around 10 will be optimal in this situation. The elbow plot is a grph that shows the WSS (Within Sum Squares) values against the number of clusters (K). To practically confirm this, we use the Silhouette Score function under sklearn's metrics module. By observing the Silhouette scores for clusters 1 to 20, we get to kneo that for cluster 8, the silhouette score is highest 0.29 approx. As we know a silhouette score close to 1 suggests that we take an optimal number of clusters.

In the last part of the project, we calculate the cluster profiles and get the z_profiles. A zprofile value of 2.58 for area means that the value is 2.58 std above the mean of that particular feature.

