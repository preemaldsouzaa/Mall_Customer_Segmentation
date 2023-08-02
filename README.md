# Mall_Customer_Segmentation
Uncovering distinct customer groups using different clustering models to oto categorize customers based on spending habits and demographics, enabling targeted marketing and business growth.

## Introduction
Customer segmentation is a vital strategy for businesses, including shopping malls, seeking to understand and cater to the diverse needs of their clientele. Mall customer segmentation involves grouping customers with similar characteristics and behavior into distinct segments. By identifying these segments, malls can personalize marketing efforts, optimize product offerings, and enhance the overall shopping experience.
In this project, we will explore the world of unsupervised learning to perform mall customer segmentation. Using various clustering algorithms, we will analyze customer data to reveal patterns and uncover valuable insights about different customer groups. The goal is to create meaningful customer segments that can guide strategic decision-making and boost customer satisfaction.
Through this project, we aim to understand the unique preferences, behaviors, and expectations of various customer segments, ultimately empowering the mall management to tailor their services and promotions to meet the specific needs of each group. Let's embark on this journey of uncovering the hidden patterns within the mall's customer data and revolutionize the way malls engage with their visitors.

## Problem Statement
The shopping mall management aims to improve customer satisfaction and optimize their marketing strategies by understanding the diverse preferences and behavior of their customers. The problem is to perform customer segmentation using unsupervised learning techniques on the mall's customer data.

## Objective:
The main objective of this project is to identify distinct customer segments based on their characteristics, shopping patterns, and preferences. By achieving effective customer segmentation, the mall management can tailor their marketing efforts, promotional campaigns, and overall services to cater to the specific needs and preferences of each customer group.

## Data Description:
The dataset contains various customer attributes such as age, gender, annual income, and spending score, which reflects the customer's purchasing behavior and spending patterns within the mall.

## Methods and Techniques:
We will employ unsupervised learning algorithms, specifically clustering techniques such as K-means, Hierarchical Clustering, or DBSCAN, to group similar customers into clusters. These clusters will represent distinct customer segments based on their shared attributes and behavior.

## Project Steps:
Data Preprocessing: Clean and preprocess the dataset, handle missing values if any, and perform feature scaling as required.

Exploratory Data Analysis (EDA): Understand the distribution and relationships among customer attributes through visualizations.

Feature Selection: Identify relevant features for customer segmentation.
 
Apply Unsupervised Learning: Implement clustering algorithms to create customer segments.

Evaluate Clustering Results: Assess the quality of the generated clusters using internal evaluation metrics.

Interpretation and Analysis: Analyze the characteristics of each customer segment to gain actionable insights.

Customer Profiling: Create detailed profiles for each customer segment, highlighting their distinct traits and preferences.

Business Recommendations: Provide strategic recommendations to the mall management based on the identified customer segments.

By successfully completing this project, the shopping mall will be equipped with valuable information about their customer base, enabling them to deliver personalized experiences, optimize marketing campaigns, and ultimately enhance customer satisfaction and loyalty.

## EDA:
The exploratory data analysis (EDA) that we have performed so far provides valuable insights into our mall customer segmentation dataset. We have analyzed various aspects of the data, including age distribution, gender distribution, annual income distribution, spending score distribution, and the relationship between different numerical variables. Additionally, we have also checked for outliers using the Z-score method.

## Model Development:
In the further step we'll apply various clustering algorithms and check which algorithm is best for our dataset. We'r going to use below algorithms:

Kmeans Clustering: K-means clustering is an unsupervised learning technique used to group unlabeled data into K clusters based on similarities in their features. The main goal is to find K centroids that represent the center of each cluster. Initially, random centroids are chosen, and the algorithm iteratively assigns data points to the nearest centroid, creating clusters. The centroids are then recalculated based on the mean of the data points in each cluster. This process continues until the centroids stabilize or a predefined number of iterations is reached. Ultimately, K-means provides cluster centroids and assigns data points to the clusters, enabling data grouping for further analysis and insights. However, it requires the number of clusters (K) to be determined beforehand.

Agglomerative Clustering: Agglomerative Hierarchical Clustering is a bottom-up hierarchical clustering algorithm used for unsupervised learning. It starts with each data point as its own cluster and then iteratively merges the closest clusters based on a chosen distance metric (e.g., Euclidean distance) until all data points belong to a single cluster or the specified number of clusters is reached. The algorithm builds a tree-like structure called a dendrogram, which represents the hierarchical clustering process.

GaussianMixture Model Clustering: Gaussian Mixture Model (GMM) is a probabilistic clustering algorithm used for unsupervised learning. It assumes that the data is generated from a mixture of multiple Gaussian distributions, each representing a cluster. GMM assigns data points to clusters based on the probabilities of belonging to each Gaussian component. It iteratively estimates the parameters of the Gaussian distributions using the Expectation-Maximization (EM) algorithm. GMM is flexible, capturing complex data structures and handling clusters of different shapes and sizes. It provides a measure of uncertainty for cluster assignments and finds applications in image segmentation, anomaly detection, data compression, and more. The main challenge is determining the appropriate number of clusters for the data. Overall, GMM is a versatile algorithm for clustering and density estimation.

DBSCAN Clustering: DBSCAN, or Density-Based Spatial Clustering of Applications with Noise, is an unsupervised machine learning algorithm used for clustering data. Unlike traditional clustering methods, DBSCAN does not require specifying the number of clusters in advance and can identify clusters of arbitrary shapes in the data. The algorithm defines three types of points: core points with sufficient nearby points, border points that are within a specified distance of core points, and noise points with no nearby points. DBSCAN iteratively expands clusters from core points, creating flexible and dense clusters while efficiently handling outliers. Its ability to automatically detect the number of clusters and handle complex datasets makes DBSCAN a valuable tool for various data analysis tasks.

We will be using Silhouette score which is a metric used to evaluate the quality of clustering in unsupervised learning. It quantifies how well-separated the clusters are and ranges from -1 to 1. A higher silhouette score indicates better-defined clusters with distinct boundaries, while negative values imply data points might be assigned to the wrong clusters. Silhouette score takes into account both cohesion within a cluster and separation from other clusters, making it a robust measure for clustering performance.

Lets see which model performs the best...

K-means achieved a silhouette score of approximately 0.5539, which suggests that the clusters are reasonably well-defined and distinct from each other.

Agglomerative clustering achieved a silhouette score of about 0.5530, indicating similar performance to K-means in terms of cluster quality.

Gaussian Mixture Model obtained a silhouette score of around 0.4270, which is lower than the previous two methods. This suggests that the clusters might be less well-defined and more overlapping in this approach.

DBSCAN produced a negative silhouette score of approximately -0.2891, which indicates that the clustering did not perform well for the given data. Negative values suggest that the data points are assigned to incorrect clusters or that the data might not be suitable for DBSCAN clustering.

Overall, based on the silhouette scores, K-means and Agglomerative clustering appear to have performed better than Gaussian Mixture and DBSCAN for this specific dataset.

## Conclusions
In conclusion, the mall customer segmentation project aimed to identify distinct customer groups based on their spending behaviors and demographics. Through exploratory data analysis, we gained valuable insights into the data, such as the distribution of customer ages, gender proportions, and the relationship between annual income and spending scores. The data revealed five clear clusters when comparing annual income and spending scores, indicating different customer segments.
We applied several clustering algorithms, including K-means, Agglomerative, Gaussian Mixture, and DBSCAN, to group the customers based on their similarities. Among these, K-means showed the best performance with a silhouette score of approximately 0.554, suggesting well-defined clusters. This clustering approach can be leveraged by the mall for targeted marketing, personalized promotions, and improving customer satisfaction.
The customer segments identified through this project can provide valuable insights for the mall management to tailor their services and offerings to meet the specific needs and preferences of each customer group. By understanding the spending behaviors and characteristics of different segments, the mall can optimize its marketing strategies and enhance customer retention and overall revenue. However, further analysis and validation are recommended to ensure the practicality and effectiveness of the segmentation in real-world scenarios.
