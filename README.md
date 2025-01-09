# Crypto Clustering
## Overview
The Crypto Clustering project explores unsupervised learning techniques to cluster cryptocurrencies based on their price performance over 24 hours and 7 days. Using K-means clustering and Principal Component Analysis (PCA), this project investigates the impact of dimensionality reduction on clustering results and visualizes the clusters effectively.

## Steps
1. Load and Preprocess Data
Load the cryptocurrency market data from crypto_market_data.csv.
Normalize the data using StandardScaler to prepare it for clustering.
2. Clustering with the Original Scaled Data
Use the elbow method to find the optimal number of clusters (k).
Perform K-means clustering using the optimal k.
Visualize the clusters using a scatter plot with price_change_percentage_24h and price_change_percentage_7d.
3. Dimensionality Reduction with PCA
Apply PCA to reduce the dataset to three principal components while retaining most of the variance.
Analyze the total explained variance of the three components.
4. Clustering with PCA Data
Use the elbow method to find the optimal number of clusters for the PCA-reduced data.
Perform K-means clustering using the optimal k.
Visualize the clusters using a scatter plot of the first two principal components (PC1 and PC2).
5. Visualization and Comparison
Compare the elbow curves and cluster visualizations of the original scaled data and PCA-reduced data using composite plots.
## Results
The following visualizations are included:

Elbow Curve:
Original Scaled Data 

![elbow_curve](https://github.com/MandeepKaurSohi/CryptoClustering/blob/main/outputs/elbow_curve.png) 


PCA Data

![elbow_pca_plot](https://github.com/MandeepKaurSohi/CryptoClustering/blob/main/outputs/elbow_pca_plot.png) 


Cluster Scatter Plots:

Original Scaled Data (price_change_percentage_24h vs. price_change_percentage_7d) 

![market_scaled_plot](https://github.com/MandeepKaurSohi/CryptoClustering/blob/main/outputs/market_scaled_plot.png) 


PCA Data (PC1 vs. PC2) 

![market_pca_plot](https://github.com/MandeepKaurSohi/CryptoClustering/blob/main/outputs/market_pca_plot.png) 


## Conclusion
This project demonstrates the effectiveness of dimensionality reduction in simplifying data for clustering while retaining key insights. The consistent identification of the optimal k across both methods highlights the robustness of K-means clustering with PCA-transformed data. Visual comparisons reveal that PCA enhances clustering efficiency and interpretability.

## Dependencies
To replicate the analysis, install the following libraries:

Python
pandas
NumPy
scikit-learn
hvPlot
holoviews
