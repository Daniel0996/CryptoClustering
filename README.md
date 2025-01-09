# CryptoClustering
Module 11 Challenge - Unsupervised Machine Learning

## Summary
Different algorithms and preprocessing techniques were interduced in Module 11.
In this challenge, we will use the K-Means algorithm and principal component analysis (PCA) to classify cryptocurrencies according to their price fluctuations across various time frames.

## Data Source
crypto_market_data.csv file in Resources folder

## Load and View the data
Load the data in the csv file into a data frame and examine the summary statistics.

## Prepare the Data
1. Use StandardScaller from the scikit-learn library to normalize the data
2. Find the best k value for the scaled dataframe using the `Elbow Method`
<p align='left'>
    <img src="images/Figure 1 - Original Scaled Data Elbow Curve.png" alt="Original Scaled Data Elbow Curve" width="400"/>
</p>

## Visualize K-Means Clusters Using Original Data
Cluster the crptocurrencies with `K-Means` with the best value of K.  Plot the clusters to visualize the data.
<p align='left'>
    <img src="images/Figure 2 - Original Scaled Data Clusters.png"
    alt="Original Scaled Data K-Means Clusters" width="400"/>
</p>

## Preprocessing Using PCA
1. Optimize clusters with `Principal Component Analysis (PCA)`
    The 3 component explained variance ratio output is 
    array([0.3719856 , 0.34700813, 0.17603793])
    <BR>
2. Find the best k value for the PCA data using the `Elbow Method`
<p align='left'>
    <img src="images/Figure 3 - PCA Data Elbow Curve.png" alt="PCA Data Elbow Curve" width="400"/>
</p>

## Visualize K-Means Clusters Using PCA Data
Cluster the crptocurrencies with `K-Means` with the best value of K.  Plot the clusters to visualize the data.
<p align='left'>
    <img src="images/Figure 4 - PCA Data Clusters.png" alt="PCA Data K-Means Clusters" width="400"/>
</p>

## Determine the Weights of Each Feature on Each Principal Component
<p align='left'>
    <img src="images/Figure 5 - PCA Component Weights .png" alt="PCA Component Weights" width="400"/>
</p>