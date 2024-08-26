# CryptoClustering - Module 11 Home Work Assignment

The data being analyzed consists of cryptocurrencies according to their price fluctuations across various timeframes. The variable **'coinid'** contains the price fluctuation information on 41 types of crypto currency. price fluctuations are diplayed for the following timebands:
* 24 hours
* 7 days
* 14 days
* 30 days
* 60 days
* 200 days 
* 1 year

  # The Objective:
The objective of this analysis is to classify crypto currency into clusters based on the given proce fluctuations.
the code is organized into the following steps:
The data is read from the csv provided in the Resources folde rof the git hub

# Analysis Details
**K means** is the first clustering process used and the Elbow graph is plotted to see that the recommended number of clusters is between 3, 4. The analysis goes with 4 as there is a steeper drop off after 4 clusters in the computed inertia values.

**PCA Analysis** condenses the dataset to represent 89.5% of the variability of the data provided into 3 principal components. the analysis arrives at a similar recommendation of 4 clusters for PCA as well. 
For each of the components, the flowing variables have the strongest positive and negative influence:
* **PCA1** - Strongest positive influence is from price_change_percentage_200d(0.594468) and the strongest negative influence is from price_change_percentage_24h (-0.416728)
* **PCA2** - Strongest positive influence is from price_change_percentage_30d(0.562182) and the strongest negative influence is from price_change_percentage_1y (-0.150789)
* **PCA3** - Strongest positive influence is from price_change_percentage_7d(0.787670) and the strongest negative influence is from price_change_percentage_60d (-0.361377)
