# K-Means Clustering

## Introduction
Clustering is an unsupervised machine learning technique that allows us to determine hidden structure in data. A clustering algorithm does not require to be trained using datasets marked with pre-defined class labels. It rather attempts to discover natural groupings by mining the clusters based on set of well defined criteria. The k-means is one of such algorithms that creates the clusters by minimizing the squared sum of distances between data points and the centeroids of their respective clusters. There also are several other approaches to clustering problem but k-means is simplest, computationaly cheapest yet highly performing. The k-means clustering has applications across several domains, the customer and market segmentation in consumer data, claim segmentation in insurance data, segmenting the stock market tickers according to past performance and anomaly detection in financial statements are only a few to name.

## Algorithm
Let K be the number of clusters specified by the user, then k-means clustering algorithm can then be summarized with following steps:
1.    Initialize algorithm by randomly assigning a cluster label (1 to K) to each data point.
2.    Compute the centroid for each of the K clusters.
3.    Calculate the Euclidean distances between each data point and each centroid.
4.    Re-assign the data point to the cluster whose centriod is closest to it.
5.    Repeat steps 2 through 5 untill centroids do not change between successive passes.

In the demonstration slide below we show stages in 1st pass of the algorithm.

    "Unlabelled Data" : Raw data as input to the algorithm (left).
    "Cluster Assignment" : Randomly assign cluster labels to data points (middle).
    "Centroid Computation" : Centroid is computed by calculating vector of feature means (right).

![kmeansassignK](https://github.com/lovedeepkaursaini/K-Means/blob/master/kmeans_step1.png)

In the following slide we show stages during one of the subsequent passes.

    "Cluster Assignment": Assign each observation to the nearest centroid (left).
    "Centroid Computation" : Recalculate the centroid like we did at 1st past (middle).
    "Final State": The state of termination of algorithm after passes saturate(right).

![kmeanscalcK](https://github.com/lovedeepkaursaini/K-Means/blob/master/kmeans_step2.png)
