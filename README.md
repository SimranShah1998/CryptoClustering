# Cryptocurrency Clustering Project

This project applies the K-means clustering algorithm and Principal Component Analysis (PCA) to classify cryptocurrencies based on their price fluctuations across various timeframes. It explores how clustering and dimensionality reduction techniques can provide insights into the cryptocurrency market.

## Objective

### The goal of this project is to:

- Normalize cryptocurrency market data for analysis.

- Use the elbow method to determine the optimal number of clusters (k).

- Cluster cryptocurrencies based on their price fluctuations.

- Reduce dimensionality using PCA to optimize clustering.

- Analyze the features that contribute most to the clustering process.

## Tools and Libraries

### The following tools and libraries were used in this project:

- Python: Programming language.

- Jupyter Notebook: For running and documenting the analysis.

- pandas: For data manipulation and analysis.

- matplotlib: For data visualization.

- scikit-learn: For implementing clustering algorithms and PCA.

## Steps

### The analysis is divided into the following sections:

1. Prepare the Data:
   
- Normalize the cryptocurrency market data using StandardScaler.

- Create a DataFrame with the normalized data.
  
2. Find the Best Value for k Using the Original Scaled Data:
   
- Apply the elbow method to determine the optimal number of clusters (k).

- Plot the inertia values to visualize the elbow point.
  
3. Cluster Cryptocurrencies Using the Original Scaled Data:
   
- Perform K-means clustering using the optimal k.
  
- Visualize the clusters using a scatter plot.
  
4. Optimize Clusters with PCA:
   
- Reduce the dimensionality of the data to three components using PCA.
  
- Calculate the total explained variance for the reduced data.
  
5. Find the Best Value for k Using the PCA Data:
   
- Repeat the elbow method on the PCA-transformed data.
  
- Compare the best k values from the original and PCA-transformed data.
  
6. Cluster Cryptocurrencies Using the PCA Data:

- Perform K-means clustering on the PCA-transformed data.
  
- Visualize the clusters using a scatter plot of the first two principal components.
  
7. Analyze Feature Weights:
   
- Determine the feature contributions to each principal component.

- Identify features with the strongest positive and negative influences.

## Results

The optimal number of clusters (k) was determined to be 4 for both the original and PCA-transformed data.

PCA explained 89.56% of the variance using three principal components.

### Key feature influences on the principal components were identified:

PC1: Strongest positive influence: price_change_percentage_200d, strongest negative influence: price_change_percentage_7d.

PC2: Strongest positive influence: price_change_percentage_30d, strongest negative influence: price_change_percentage_24h.

PC3: Strongest positive influence: price_change_percentage_14d, strongest negative influence: price_change_percentage_7d.

