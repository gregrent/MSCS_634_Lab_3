# Lab 3: Clustering Analysis Using K-Means vs K-Medoids Algorithms

## Purpose of the Lab
The purpose of this lab was to explore and compare two clustering techniques: **K-Means** and **K-Medoids** using the Wine dataset from the sklearn library. The objective was to understand how each algorithm groups data, evaluate their performance using clustering metrics, and visualize the differences between their results. This lab also helped reinforce the importance of data preprocessing, evaluation metrics, and visualization in clustering tasks.

---

## Key Insights from Clustering Results
- Both K-Means and K-Medoids were applied with **k = 3**, matching the number of wine classes in the dataset.
- **K-Means produced better clustering performance** than K-Medoids.
- The **Silhouette Score** for K-Means was slightly higher, indicating more compact and well-separated clusters.
- The **Adjusted Rand Index (ARI)** for K-Means was significantly higher, meaning its clusters aligned more closely with the true class labels.
- Visualizations showed that K-Means formed clearer and more structured clusters, while K-Medoids produced slightly less accurate groupings.

Overall, the results suggest that the Wine dataset has characteristics that favor K-Means, such as relatively well-separated and spherical clusters.

---

## Challenges and Decisions
- The main challenge was the **missing K-Medoids library**, which required installing the `scikit-learn-extra` package.
- Another key decision was to **standardize the dataset** using z-score normalization to ensure that all features contributed equally to the clustering process.
- **PCA was used for visualization** so that high-dimensional data could be represented in a 2D scatter plot for easier comparison.
- The number of clusters (**k = 3**) was chosen based on the known number of classes in the dataset.

---

## Conclusion
This lab demonstrated how different clustering algorithms can produce varying results on the same dataset. K-Means showed better performance on the Wine dataset, while K-Medoids remains useful for datasets with noise or outliers. The lab highlighted the importance of preprocessing, evaluation metrics, and visual analysis when performing clustering.
