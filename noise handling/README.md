
For the Silhoutte Coefficient (SC) computation with outliers, we are considering the case where we compute the SC on the data excluding the outliers. We want to understand how much the outliers affect the clustering of the actual inliers. So we are considering the followinging steps for the noisy data experiment:

1. Add outliers to the data
2. Run clustering (kmeans or ClAM)
3. After prototypes are learned, and clusters are assigned, remove all the outliers in the data.
4. Compute the quality (SC) of the cluster assignments of the inliers.

This means, in the above plots, Clean.png, Kmeans_clean.png & ClAM_clean.png are for the case where there is no outliers in the data. We add only three outliers with the original data points that is referred by Noisy.png. Kmeans_noisy.png & Clam_noisy.png are referring the clustering quality where we remove the outliers after learning the prototypes and assigning labels to the data points which help to understand how much the outliers affect the clustering quality of the actual inliers. 
