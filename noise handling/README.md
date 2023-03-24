<!-- <div style="display:flex;justify-content:center;align-items:center;">
  <img src="Clean.png" height="200px" style="margin-right:10px;">
  <img src="Kmeans_clean.png" height="200px" style="margin-right:10px;">
  <img src="ClAM_clean.png" height="200px">
</div>

<div style="display:flex;justify-content:center;align-items:center;">
  <img src="Noisy.png" height="200px" style="margin-right:10px;">
  <img src="Kmeans_noisy.png" height="200px" style="margin-right:10px;">
  <img src="ClAM_noisy.png" height="200px">
</div> -->

<p align="center">
  <img src="Clean.png" height="250px" hspace="20">
  <img src="Kmeans_clean.png" height="250px" hspace="20">
  <img src="ClAM_clean.png" height="250px" hspace="20">
</p>

<p align="center">
  <img src="Noisy.png" height="250px" hspace="20">
  <img src="Kmeans_noisy.png" height="250px" hspace="20">
  <img src="ClAM_noisy.png" height="250px" hspace="20">
</p>

To evaluate the robustness to outliers, we consider a toy-example with two clusters and we study the performance of kmeans and ClAM. We first add outliers to an example dataset. Clean.png refers to the original dataset and Noisy.png refers to the dataset with outliers (which are shown in magenta color).

Next, we run both Kmeans and ClAM on the both the original and noisy datasets (Kmeans_clean.png and ClAM_clean.png refer  to the results on the original dataset, and Kmeans_noisy.png & Clam_noisy.png refer to the results on the noisy dataset).

We then compute the clustering quality via SC/NMI and ARI metrics. However, for the noisy dataset, we compute the metrics only on the inliers (i.e., excluding the outliers), to see how much the outliers affect the clustering quality of the actual inliers.

The following table shows the performance of kmeans and ClAM as noise (outliers) is added to the data:
| Method | SC (no outliers) | SC (with outliers) |
| --- | --- | --- |
| kmeans | 0.511 | 0.477 |
| ClAM | 0.531 | 0.531 |


The results indicate that, as expected, the addition of outliers reduces the clustering quality of kmeans. However, ClAM is able to cluster the data points correctly even with outliers (with NMI & ARI both equal to 1.0), showing that it can be more robust to the outliers. 

