# Cryptocurrency Clustering Analysis

This project involves clustering cryptocurrencies based on their market data using Python libraries such as `pandas`, `hvplot`, and `scikit-learn`. The clustering analysis is performed both on the original data and on data optimized using Principal Component Analysis (PCA).

## Project Structure

The project is structured as follows:

- `crypto_market_data.csv`: The dataset containing cryptocurrency market data.
- `Crypto_Clustering.ipynb`: Jupyter notebook containing the complete analysis and code.

## Requirements

To run the analysis, you need the following Python libraries:

- `pandas`
- `hvplot`
- `scikit-learn`

You can install these dependencies using the following command:

```bash
pip install pandas hvplot scikit-learn
```

## Analysis Steps
1. Load and Prepare the Data:
  - Load the data into a Pandas DataFrame.
  - Normalize the data using StandardScaler.
2. Determine the Optimal Number of Clusters (k):
  - Use the Elbow method to find the best value of k for the original data.
  - Plot the Elbow curve and identify the optimal k.
3. Cluster Cryptocurrencies Using K-Means:
  - Initialize and fit the K-Means model with the optimal k.
  - Predict clusters and visualize them using hvPlot.
4. Optimize Clusters with PCA:
  - Reduce the data to three principal components using PCA.
  - Determine the optimal k for the PCA data using the Elbow method.
  - Cluster the PCA data using K-Means and visualize the results.
5. Compare Clustering Results:
  - Contrast the clustering results from the original data and PCA data.
  - Analyze the impact of using fewer features for clustering.
    
## Key Findings
  - The optimal number of clusters (k) may differ between the original data and the PCA-optimized data.
  - Using PCA to reduce the number of features can lead to more distinct and interpretable clusters.

## Visualizations
The project includes several visualizations:
  - Elbow curves for determining the optimal k.
  - Scatter plots of the clusters based on the original data.
  - Scatter plots of the clusters based on the PCA data.

## Conclusion
The project demonstrates how dimensionality reduction using PCA can impact clustering results, leading to potentially more meaningful and interpretable clusters.
