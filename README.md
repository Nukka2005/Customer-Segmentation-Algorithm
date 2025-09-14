# K-Means Clustering for Customer Segmentation
#
## Overview
# This repository contains a Jupyter Notebook implementing K-Means clustering for customer segmentation using the Mall Customers dataset. The goal is to group customers based on their annual income and spending score to identify patterns and segments for targeted marketing strategies.
#
# This is an unsupervised machine learning assignment focused on:
# - Data preprocessing (loading, handling missing values, standardization).
# - Applying K-Means clustering.
# - Determining the optimal number of clusters using the Elbow Method.
# - Visualizing clusters and centroids.
#
## Dataset
# The dataset used is **Mall_Customers.csv** from Kaggle:  
# [Customer Segmentation Tutorial in Python](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python)
#
# - **Features used for clustering**:
#   - Annual Income (k$): Annual income in thousands of dollars.
#   - Spending Score (1-100): Score based on spending behavior.
# - **Ignored features**: Gender, Age, CustomerID (not relevant for this clustering task).
# - **Size**: 200 records.
# - No target variable (unsupervised learning).
#
# Download the dataset and place it in the project directory as `Mall_Customers.csv`.
#
## Requirements
# - Python 3.x
# - Libraries (install via `pip install -r requirements.txt`):
#   - pandas
#   - numpy
#   - scikit-learn (for KMeans and StandardScaler)
#   - matplotlib
#   - seaborn (for visualizations)

# The notebook performs:
# - Data loading and exploration.
# - Feature standardization using `StandardScaler`.
# - K-Means clustering with initial `k=5`.
# - Elbow Method to find optimal `k` (plots WCSS vs. number of clusters).
# - Cluster visualization (scatter plot of clusters and centroids).
# - Evaluation of cluster centers for different `k` values.
#
## Results
# - **Optimal Clusters**: Determined to be 5 using the Elbow Method, where the rate of decrease in inertia (WCSS) slows significantly.
# - **Visualizations**:
#   - Elbow plot showing WCSS for k=1 to 10.
#   - Scatter plot of customer segments based on Annual Income vs. Spending Score, colored by cluster, with centroids marked.
# - **Insights**: Customers are segmented into groups like high-income high-spenders, low-income low-spenders, etc., which can inform business strategies.
#
# Example output from the notebook:
# - Best number of clusters: 5
# - Cluster centroids and assignments are printed and visualized.
#
## Files
# - `K_Means_Clustering.ipynb`: Main Jupyter Notebook with code and explanations.
# - `Mall_Customers.csv`: Dataset (not included; download from Kaggle).
# - `requirements.txt`: List of Python dependencies.
# - `README.md`: This file.

## Acknowledgments
# - Dataset provided by Kaggle user [vjchoudhary7](https://www.kaggle.com/vjchoudhary7).
# - Built using scikit-learn for clustering and matplotlib/seaborn for visualizations.
