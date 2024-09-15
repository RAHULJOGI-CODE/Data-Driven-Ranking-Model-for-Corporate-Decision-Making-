# Data-Driven-Ranking-Model-for-Corporate-Decision-Making-
A Machine Learning model to assist corporate decision-making by clustering and ranking key performance metrics.

This repository contains a Data-Driven Ranking Model designed to assist corporate decision-making by clustering and ranking key performance metrics from datasets. The model leverages machine learning techniques to categorize data points into meaningful clusters, rank them based on business-defined criteria, and provide actionable insights for decision-makers.
Note : I choose Cricket franchises as a corporate and Designed this model for ranking of cricket players so that franchises can startigise thier team building .
This model with minor changes can be imolemented to many corporate companies decsion making like in Swiggy , HR's can use to cluster applicants etc.., 

### Features
KMeans Clustering: Automatically clusters datasets based on optimal number of clusters determined by silhouette scores.
Dynamic Grading System: Ranks clusters using customizable criteria such as performance indicators (e.g., runs, strike rate, wickets).
Feature Scaling: Preprocessing techniques to ensure accurate clustering results.
Cluster Visualization: Graphical representation of clusters and centroids for easy interpretation.
Automated Reporting: Generates rankings and insights in CSV or graphical format for business use.

### Requirements
Python 3.x
Libraries:
pandas
numpy
scikit-learn
matplotlib
seaborn

Install the required dependencies using the following command:
pip install -r requirements.txt

### How to Use
Load Data: Input CSV datasets using the provided load_data() function.
Feature Scaling: The data will be automatically scaled for clustering.
Cluster Analysis: The model will determine the best number of clusters and perform KMeans clustering.
Ranking: Clusters are ranked based on the defined grading system, which can be modified according to specific business needs.
Visualization: Use the plot_clusters() function to visualize the clusters and centroids.
Export Results: Save the ranked clusters and insights in CSV format for further analysis.

### Code Overview
data_driven_ranking.py: Contains the core functionality for loading data, clustering, grading, and ranking.
visualization.py: Handles the visualization of clusters using Matplotlib and Seaborn.
utils.py: Utility functions for data preprocessing, scaling, and report generation.

### Customization
You can modify the ranking criteria within the grading_function() in data_driven_ranking.py. The default behavior is:

For performance datasets (e.g., sports data), ranking is based on average of runs + strike rate.
For other datasets with attributes like wickets, it uses the average of dots + wickets.


### Future Work
Integrating additional clustering techniques (e.g.,other than  DBSCAN, Hierarchical Clustering).
Extending the model to handle time-series data for trend analysis.
Adding a web interface for easier interaction with the model.

### Contribution:
This Model is developed by me (Rahul Jogi)  and my friends Swapnith,Leela Naresh & Bhavika Reddy.

