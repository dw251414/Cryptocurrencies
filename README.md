# Cryptocurrencies
   ## Resources
   - Data Source: [crypto_data.csv](https://github.com/dw251414/Cryptocurrencies/blob/main/Resources/crypto_data.csv), [CryptoCompare](https://min-api.cryptocompare.com/data/all/coinlist)
   - Software: Python 3.9.2, Anaconda Navigator 1.9.12, Conda 4.8.4, Jupyter Notebook 6.0.3
## Analysis Overview
The purpose of this project is to use unsupervised machine learning to analyze a database of cryptocurrencies and create a report including the traded cryptocurrencies classified by group according to their features. In practice, this classification report could be used by an investment bank to propose a new cryptocurrency investment portfolio to its clients.
<br><br>

#### Methods for the analysis:

---
- preprocessing the database
- reducing the data dimension using Principal Component Analysis
- clustering cryptocurrencies using K-Means
- visualizing classification results with 2D plots

## Results
After preprocessing and cleaning, we have a total of 532 tradable cryptocurrencies.
<br><br>

### Clustering Cryptocurrencies using K-Means - Elbow Curve
Deployed unsupervised machine learning to identify clusters of the cryptocurrencies. The elbow curve below using the K-Means method iterating on k values from 1 to 10.

---
<p align="center">
    <img width="1082" alt="Screen Shot 2021-08-28 at 11 33 45 PM" src="https://user-images.githubusercontent.com/82069038/131237421-5042df05-6655-415b-849d-c8c8eea70af6.png">
</p>
The best k value appears to be 4 so we would conclude on an output of 4 clusters to categorize the crytocurrencies.
<br><br>

## Visualizing Cryptocurrencies Results

### 2D-Scatter plot with clusters

---
<p align="center">
    <img width="1278" alt="Screen Shot 2021-08-28 at 11 34 37 PM" src="https://user-images.githubusercontent.com/82069038/131237432-c8b8011e-89a9-4916-a668-d7a13b43fa60.png">
</p>
This 2-D scatter plot was obtained using the PCA algorithm to reduce the crytocurrencies dimensions to two principal components. This plot shows the distribution and the four clusters of cryptocurrencies. Amongst other variability, we're able to identify outliers like the unique cryptocurrency in the class #2.
<br><br>

### Tradable Cryptocurrencies Table

---
<p align="center">
    <img width="762" alt="Screen Shot 2021-08-28 at 11 15 06 PM" src="https://user-images.githubusercontent.com/82069038/131237288-4063772f-ec2b-4b7a-94d1-c293cbd84855.png">
</p>
Most of the cryptocurrencies are part of class #0 and #1.The snapshot above shows that BitTorrent is the only cryptocurrency in class #2.
<br><br>

### 2D-Scatter plot with TotalCoinMined vs TotalCoinSupply

---
<p align="center">
    <img width="1169" alt="Screen Shot 2021-08-28 at 11 34 12 PM" src="https://user-images.githubusercontent.com/82069038/131237444-a6d72fb0-0016-4603-ae1a-c91b10fed8f6.png">
</p>
The PCA algorithm identifies class as a parameter, and is the better visualization.
<br><br>

## Summary
We have identified the classification of 532 cryptocurrencies based on feature similarities. To determine their performance along with potential IB interest, further analysis on unique group traits should be conducted.
