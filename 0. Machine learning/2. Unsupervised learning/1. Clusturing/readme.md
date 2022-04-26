## About

- In clusturing the aim is to segregate groups with similar traits and assign them into clusters.

- Clustering has a myriad of uses in a variety of industries.

- Many clustering algorithms work by computing the similarity between all pairs of examples.

- This means their runtime increases as the square of the number of examples , denoted as in complexity notation. algorithms are not practical when the number of examples are in millions.

- The k-means algorithm, which has a complexity of , meaning that the algorithm scales linearly with .

> **Types of Clustering**

> > **Centroid-based Clustering**

- Centroid-based clustering organizes the data into non-hierarchical clusters, in contrast to hierarchical clustering defined below.
- k-means is the most widely-used centroid-based clustering algorithm.
- Centroid-based algorithms are efficient but sensitive to initial conditions and outliers.

> > **Density-based Clustering**

- Density-based clustering connects areas of high example density into clusters.
- This allows for arbitrary-shaped distributions as long as dense areas can be connected.
- These algorithms have difficulty with data of varying densities and high dimensions

> > **Distribution-based Clustering**

- This clustering approach assumes data is composed of distributions.
- As distance from the distribution's center increases, the probability that a point belongs to the distribution decreases.
- The bands show that decrease in probability. When you do not know the type of distribution in your data, you should use a different algorithm.

> > **Hierarchical Clustering**

- Hierarchical clustering creates a tree of clusters. - Hierarchical clustering, not surprisingly, is well suited to hierarchical data, such as taxonomies

> Some common applications for clustering include the following:

- market segmentation
- social network analysis
- search result grouping
- medical imaging
- image segmentation
- anomaly detection

## K Means Clustering

- K means is an iterative clustering algorithm that aims to find local maxima in each iteration.

> This algorithm works in these 5 steps :

- Specify the desired number of clusters K : Let us choose k=2 for these 5 data points in 2-D space.
- Randomly assign each data point to a cluster : Let’s assign three points in cluster 1 shown using red color and two points in cluster 2 shown using grey color.
- Compute cluster centroids : The centroid of data points in the red cluster is shown using red cross and those in grey cluster using grey cross.

> Re-assign each point to the closest cluster centroid :

- Note that only the data point at the bottom is assigned to the red cluster even though its closer to the centroid of grey cluster. Thus, we assign that data point into grey cluster.

> Re-compute cluster centroids :

- Now, re-computing the centroids for both the clusters.

> Repeat steps 4 and 5 until no improvements are possible :

- Similarly, we’ll repeat the 4th and 5th steps until we’ll reach global optima. When there will be no further switching of data points between two clusters for two successive repeats.

- It will mark the termination of the algorithm if not explicitly mentioned.
  **Use cases**

- Recommender system
- Targeted marketing
- Customer segmentation
