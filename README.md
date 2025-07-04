# Task-8-Clustering-with-K-Means

1.Load and visualize dataset (optional PCA for 2D view).

2.Fit K-Means and assign cluster labels.

3.Use the Elbow Method to find optimal K.

4.Visualize clusters with color-coding.

5.Evaluate clustering using Silhouette Score.

---
# Objective: 
Perform unsupervised learning with K-Means clustering.

---
# Tools:
Scikit-learn, Pandas, Matplotlib

---

# code explainaton

---

Step 1: Import Required Libraries

Libraries like Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn are used.

These help in data manipulation, scaling, clustering, visualization, and evaluation.



---

 Step 2: Load Dataset

The dataset Mall_Customers.csv is loaded using Pandas.

This dataset typically contains customer information like Age, Gender, Annual Income, and Spending Score.



---

 Step 3: Basic Exploration

Print the first few rows to understand the data structure.

Use .info() to check for missing values or data types.



---

Step 4: Feature Selection

Select the relevant features for clustering.

In this case: Annual Income (k$) and Spending Score (1-100) are chosen for simplicity and better 2D visualization.



---

 Step 5: Standardize the Data

StandardScaler is used to scale the features.

This ensures that all variables contribute equally to the clustering.



---

 Step 6: Elbow Method

Run KMeans clustering for a range of cluster values (e.g., 1 to 10).

Record the inertia (sum of squared distances from points to their assigned cluster center).

Plot number of clusters vs inertia.

The “elbow point” in the graph indicates the optimal number of clusters.



---

 Step 7: Fit KMeans with Optimal K

Based on the elbow graph (usually K=5 for this dataset), the KMeans algorithm is run again with that optimal number of clusters.

This assigns a cluster label (0 to K-1) to each data point.



---

 Step 8: Assign Cluster Labels

Add the predicted cluster labels as a new column to the original DataFrame.

This helps in later visualization and analysis.



---

 Step 9: Visualize Clusters

Create a scatter plot using Annual Income and Spending Score, color-coded by cluster.

Also, plot the centroids of each cluster using a distinct marker (e.g., yellow X).

This gives a visual understanding of how customers are segmented.



---
 Step 10: Evaluate with Silhouette Score

Calculate the Silhouette Score, which measures how well each point fits within its cluster.

Values range from -1 to 1.

A score closer to 1 means well-defined clusters.


This is used to validate the clustering quality.



---

Step 11: Optional PCA for 2D Visualization

Use Principal Component Analysis (PCA) to reduce the data to 2D.

Plot the data again using PCA components with clusters colored.

This helps in visualizing higher-dimensional clustering in 2D.



---
