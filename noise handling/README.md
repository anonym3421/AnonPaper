
For the purpose of this experiment, we are considering the case where we compute the clustering metrics (SC/NMI/ARI) on the data excluding the outliers. We want to understand how much the outliers affect the clustering of the actual inliers. So we are considering the followinging steps for this particular experiment:

1. Add outliers to the data
2. Run clustering (kmeans or ClAM)
3. After prototypes are learned, and clusters are assigned, remove all the outliers from the data.
4. Compute the quality (SC/NMI/ARI) of the cluster assignments of the inliers.

This means, in the above plots, Clean.png, Kmeans_clean.png & ClAM_clean.png are for the case where there is no outlier in the data. We add only three outliers (colored in magenta) with the original data points and create a new dataset (Noisy.png). Kmeans_noisy.png & Clam_noisy.png are referring the clustering where we remove the outliers after learning the prototypes and assigning labels to each of the data points which indicates how much the outliers affect the clustering quality of the actual inliers. 
