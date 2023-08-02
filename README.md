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
Kmeans Clustering
Agglomerative Clustering
GaussianMixture Model based clustering
DBSCAN Clustering

## Conclusions
In conclusion, the mall customer segmentation project aimed to identify distinct customer groups based on their spending behaviors and demographics. Through exploratory data analysis, we gained valuable insights into the data, such as the distribution of customer ages, gender proportions, and the relationship between annual income and spending scores. The data revealed five clear clusters when comparing annual income and spending scores, indicating different customer segments.
We applied several clustering algorithms, including K-means, Agglomerative, Gaussian Mixture, and DBSCAN, to group the customers based on their similarities. Among these, K-means showed the best performance with a silhouette score of approximately 0.554, suggesting well-defined clusters. This clustering approach can be leveraged by the mall for targeted marketing, personalized promotions, and improving customer satisfaction.
The customer segments identified through this project can provide valuable insights for the mall management to tailor their services and offerings to meet the specific needs and preferences of each customer group. By understanding the spending behaviors and characteristics of different segments, the mall can optimize its marketing strategies and enhance customer retention and overall revenue. However, further analysis and validation are recommended to ensure the practicality and effectiveness of the segmentation in real-world scenarios.
