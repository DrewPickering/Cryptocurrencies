# Challenge – Accountability Accounting; Cryptocurrencies

## Overview

Use unsupervised learning to analyze data on the cryptocurrencies traded on the market.

Use unsupervised learning to group cryptocurrencies, on a clustering algorithm to help determine about investing opportunities. Use data visualizations to show findings.

## Objectives

Prepare the data for dimensions reduction with PCA and clustering using K-means.

Reduce data dimensions using PCA algorithms from sklearn.

Predict clusters using cryptocurrencies data using the K-means algorithm form sklearn.

Create some plots and data tables to present your results.

## Data Prep

1.	Remove all cryptocurrencies that aren’t trading.
2.	Remove all cryptocurrencies that don’t have an algorithm defined.
3.	Remove the IsTrading column.
4.	Remove all cryptocurrencies with at least one null value.
5.	Remove all cryptocurrencies without coins mined.
6.	Store the names of all cryptocurrencies on a DataFramed named coins_name, and use the crypto_df.index as the index for this new DataFrame.
7.	Remove the CoinName column.
8.	Create dummies variables for all of the text features, and store the resulting data on a DataFrame named X.
9.	Use the StandardScaler from sklearn to standardize all of the data from the X DataFrame. Remember, this is important prior to using PCA and K-means algorithms.

## Reducing Data Dimensions Using PCA

Use the PCA algorithm from sklearn to reduce the dimensions of the X DataFrame down to three principal components.

## Clustering Cryptocurrencies Using K-means

1.	Create an elbow curve to find the best value for K.
2.	Run the K-means algorithm to predict the K clusters for the cryptocurrencies’ data. 
3.	Create a new DataFrame named “clustered_df,” that includes the following columns: Algorithm, ProofType, TotalCoinsMined, TotalCoinSupply, PC 1, PC 2, PC 3, CoinName, and Class.

## Visualizing Results

1.	Plot the clusters in a 3D scatter plot 
2.	Create a data table with all the current tradable cryptocurrencies. 
3.	Create a scatter plot to present the clustered data about cryptocurrencies contrasting the number of available coins versus the total number of mined coins. 

## Findings

Accountability Accounting is seeking to invest in crypto currencies, and the unsupervised machine learning algorithms help to identify those currencies that are established versus the many that are still in some stage of development.  

Our original dataset had 1,252 cryptocurrencies, which was quickly reduced down to 1,144 that are actually trading, Then, after dropping the cryptocurrencies that had null values we narrowed the field to 685.  Some of these had not mined any coins or fractions of coins, and we filtered down to 532 currencies that had mined coins. 

The visualizations display that many of the cryptocurrencies have mined very few coins, relative to coins available.  Accountability, accounting can interpret the data from the visualization and choose coins that are actively being mined and perhaps they will invest in a few of the early stage currencies with the same algorithms as some of the proven currencies.
