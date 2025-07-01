## Clustering Analysis with DBSCAN, K-Means, and Hierarchical Clustering 

## Objective 

This assignment focuses on applying and analyzing the DBSCAN clustering algorithm, comparing its performance against K-Means and Hierarchical Clustering. Through hands-on experimentation with various datasets, the project aims to: 

Understand DBSCAN’s mechanics and how it identifies clusters and handles noise. 
Highlight key differences between DBSCAN, K-Means, and Hierarchical Clustering. 
Evaluate performance through visualizations and comparative analysis. 

## DBSCAN Algorithm Overview:  

## Cluster Identification 

DBSCAN groups data points based on the density of surrounding points. A point is classified as: 

Core point: Has at least min_samples neighbors within radius eps. 
Border point: Is within eps of a core point but doesn’t have enough neighbors to be a core itself. 
Noise point: Are the outliers. 

## Key Parameters 

eps (ε): Defines the radius of the neighborhood around a data point. Choosing an appropriate eps is crucial: 
Too small → many points classified as noise. 
Too large → distinct clusters may merge. 
min_samples: Minimum number of points (including the point itself) required to form a dense region. 

## Strengths 

Captures arbitrarily shaped clusters. 
Handles outliers effectively. 
No need to pre-define the number of clusters. 

## Limitations 
Performs poorly with varying density clusters. 
Struggles in high-dimensional spaces.  

## Datasets Used 

make_moons(n_samples=300, noise=0.05): Non-spherical, well-separated clusters → good for DBSCAN. 
make_blobs(n_samples=300, centers=3, cluster_std=[1.0, 2.5, 0.5]): Varying densities → shows DBSCAN’s limitations. 

## Analysis 

Where DBSCAN Excels 
Detecting clusters of arbitrary shape. 
Filtering out noise effectively. 
No need to specify number of clusters. 

Where DBSCAN Struggles 
Clusters with different densities: A single eps can’t handle all variations. 
Parameter tuning: Sensitive to choice of eps and min_samples. 
High-dimensional data: Distance metrics become less meaningful. 


## References 

Demo of DBSCAN clustering algorithm. (n.d.) Scikit-Learn. https://scikit-learn.org/stable/auto_examples/cluster/plot_dbscan.html 
GeeksforGeeks. (2019). DBSCAN Clustering in ML Density based clustering. GeeksforGeeks. https://www.geeksforgeeks.org/machine-learning/dbscan-clustering-in-ml-density-based-clustering/ 
