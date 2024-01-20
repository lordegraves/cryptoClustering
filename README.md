# Cryptocurrency Market Analysis Tool

## Overview

This tool analyzes cryptocurrency market data using clustering and principal component analysis (PCA). It normalizes market data, applies K-Means clustering, and uses PCA for dimensionality reduction to identify patterns and groupings in cryptocurrency market behaviors.

## Dependencies

- Python 3
- Pandas
- scikit-learn (KMeans, PCA, StandardScaler)

## Data

The program expects a CSV file named `crypto_market_data.csv` in a `Resources` folder. This file should contain cryptocurrency market data with a `coin_id` column as the index.

## Features

1. **Data Loading and Normalization**: Loads market data and normalizes selected features using `StandardScaler`.

2. **K-Means Clustering**: Applies K-Means clustering to group cryptocurrencies based on market behaviors. Includes an Elbow Curve plot to determine the optimal number of clusters.

3. **Principal Component Analysis**: Reduces the dimensionality of the data to three principal components and applies K-Means clustering on this reduced data.

4. **Visualization**: Generates scatter plots to visualize the clustering results based on market changes and PCA components.

## Usage

1. **Load Data**: Load the cryptocurrency market data.
2. **Normalize Data**: Standardize the features for clustering.
3. **K-Means Clustering**: Identify clusters in the market data.
4. **PCA Application**: Apply PCA and redo clustering on the transformed data.
5. **Visualization**: Visualize the results using scatter plots.

## Notes

- Ensure that the `crypto_market_data.csv` file is correctly formatted and placed in the `Resources` directory.
- Adjust the range of `k` values in the K-Means algorithm as needed for different datasets.
