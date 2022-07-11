# Cryptocurrencies
## Analysis Overview
The purpose of this project is to use unsupervised machine learning to analyze a database of cryptocurrencies and create a report including the traded cryptocurrencies classified by group according to their features.
This classification report could be used by an investment bank to propose a new cryptocurrency investment portfolio to its clients.
We use the following methods for the analysis:

preprocessing the database,
reducing the data dimension using Principal Component Analysis,
clustering cryptocurrencies using K-Means,
visualizing classification results with 2D and 3D scatter plots.

## Results
### Clustering Cryptocurrencies using K-Means - Elbow Curve
We don't know what would be the output of the analysis so we are using unsupervised machine learning to identify clusters of the cryptocurrencies.
We produced the elbow curve below using the K-Means method iterating on k values from 1 to 10.

<img width="551" alt="Screen Shot 2022-07-10 at 9 58 12 PM" src="https://user-images.githubusercontent.com/100812308/178174548-e399cd48-d3f3-4307-a67c-fc2e5296d1d0.png">

The best k value appears to be 4 so we would conclude on an output of 4 clusters to categorize the crytocurrencies.

### Visualizing Cryptocurrencies Results

#### 3D-Scatter plot with clusters
This 3-D scatter plot was obtained using the PCA algorithm to reduce the crytocurrencies dimensions to three principal components.

<img width="767" alt="Screen Shot 2022-07-10 at 10 00 47 PM" src="https://user-images.githubusercontent.com/100812308/178174709-b98513ed-b51e-48b0-9d64-a5faf61d2ed2.png">


#### 2D-Scatter plot with clusters

This 2-D scatter plot was obtained using the PCA algorithm to reduce the crytocurrencies dimensions to two principal components.

Both these scatter plots show the distribution and the four clusters of cryptocurrencies.
We can identify the outliers like the unique cryptocurrency in the class #2.

<img width="519" alt="Screen Shot 2022-07-10 at 10 02 27 PM" src="https://user-images.githubusercontent.com/100812308/178174838-4abd4c2d-0c9e-4854-bfb1-59e955947f77.png">

#### Tradable Cryptocurrencies Table

<img width="624" alt="Screen Shot 2022-07-10 at 10 04 43 PM" src="https://user-images.githubusercontent.com/100812308/178175038-f1622a46-3d38-43b4-9375-d5ab5f7564ec.png">


Most of the cryptocurrencies are part of class #0 and #1.
The snapshot above shows that BitTorrent is the only cryptocurrency in class #2.

#### 2D-Scatter plot with TotalCoinMined vs TotalCoinSupply
Plotting the scatter plot from two cryptocurrency features directly does not efficiently segregate the different classes. Then using the PCA algorithm is the right method for better visualizations.

<img width="553" alt="Screen Shot 2022-07-10 at 10 11 12 PM" src="https://user-images.githubusercontent.com/100812308/178175747-68a8fe2f-0947-424a-a6b7-cec6679ff3f8.png">

## Summary
We have identified the classification of 532 cryptocurrencies based on similarities of their features.
Particularities of each group need to be analyzed to determined their performance and potential interest for the investment bank's clients.
