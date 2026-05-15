# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Load the dataset and select the relevant features for clustering (Annual Income and Spending Score).
  
2. Initialize the number of clusters (K) and apply the K-Means algorithm to the dataset.

3. Randomly assign initial centroids and group data points based on nearest centroid.

4. Recalculate centroids by taking the mean of all points in each cluster and repeat until convergence.

5. Visualize the clustered data and final centroids using a scatter plot.
 

## Program:
```
/*

Developed by: N.Gowsalya
RegisterNumber:  212225230085

import pandas as pd
import matplotlib.pyplot as plt
from sklearn.cluster import KMeans

data = pd.read_csv("C:/Downloads/Mall_Customer.csv")

X = data.iloc[:, [3, 4]].values

kmeans = KMeans(n_clusters=5, random_state=0)

y_kmeans = kmeans.fit_predict(X)

plt.scatter(X[:, 0], X[:, 1], c=y_kmeans, s=50)
plt.scatter(kmeans.cluster_centers_[:, 0],
            kmeans.cluster_centers_[:, 1],
            s=200,
            marker='X')

plt.xlabel("Annual Income")
plt.ylabel("Spending Score")
plt.title("Customer Segmentation using K-Means")

plt.show()
*/
```

## Output:
<img width="827" height="566" alt="Screenshot 2026-05-15 144433" src="https://github.com/user-attachments/assets/76615d54-bc52-4751-85f4-890a4c9c6995" />



## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
