# Module 19 (CryptoClustering)

## **Overview**
This project focuses on utilizing unsupervised machine learning techniques like K-Means clustering and Principal Component Analysis (PCA) to analyze cryptocurrency market data. The goal is to determine whether cryptocurrencies can be group based on their price changes over 24 hours and 7 dats.
The challenge covers:
1. Prepare the data by loading and normalize the cryptocurrency market data.
2. Find the Optimal K using the elbow method to determine the best number of clusters.
3. Apply K-Means clustering on the scaled data by initializing a K-Means model with the best k value, predict cluster assignments and visualize the clusters using hvPlot scatter plot.
4. Perform Principal Component Analysis (PCA) to reduce data features to three PCs, evaluate the explained variance and create a new PCA DataFrame. 
5. Run the elbow method again to determine the best k value for PCA data. Apply K-Means clustering on reduced PCA features and visualize the results using hvPlot scatter plot
6. Create composite visualization to compare clustering on orginial vs. PCA-reduced data.

## **Technologies Used**
- Python 
- Google Colab
- Pandas
- sklearn 
    - K-Means Clutering
    - Principal Component Analysis (PCA)
    - StandardScaler
- hvPlot
- HoloViews
- Matplotlib/Bokeh


CryptoClustering/
│   crypto_market_data.csv        # Cryptocurrency market dataset
│   Crypto_Clustering.ipynb       # Jupyter Notebook with code implentation
│   README.md           # Project documentation (this file)

## **Setup Instructions**
1. **Clone the Repository:**
Clone the GitHub repository and navigate into the project directory

2. **Install the Dependencies:**
hvPlot, Holoviews and scikit-learn are installed 

3. **Load and Explore the Data :**
Load the crypto market data into a Pandas DataFrame to display summary statistics and visualize trends in price changes.

4. **Prepare the Data:** 
Normalize the data using StandardScaler() and create a scaled DataFrame and set coin_id as the index

5. **Find the Best K Using the Elbow Method:**
- Create a range of k values from 1 to 11. Compute the inertia for each k value and store it.
- Plot the Elbow Curve to identify the optimal number of clusters 

6. **Clustering with K-Means:**
- Initialize and fit the K-Means models using the optimal k value.
- Predict cluster labels and add them to the DataFrame
- Generate a scatter plot of clusters using hvPlot.

7. **Optimize Clusters with PCA:**
- Apply PCA to reduce the feature dimensions from multiple price change columns to three principal components.
- Check the explained variance to ensure data retention 

8. **Find the Best k using PCA Data:**
Rerun the Elbow method on the PCA-transformed data and confirm the best value for k.

9. **Use PCA Data to perform K-Means Clustering:**
- Initialize and fit K-Means on the PCA-transformed data.
- Predict cluster labels and visualize using hvPlot

10. **Compare the Results:**
Create composite visualization to compare elbow curves and cluster plots on orginial vs. PCA-reduced data.

