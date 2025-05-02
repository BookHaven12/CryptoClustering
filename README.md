# CryptoClustering
This project utilizes unsupervised machine learning techniques to predict changes to cryptocurrencies in relation to 24-hour and 7 day price changes. By using K Means clustering and Principal Component Analysis (PCA), the goal is to identify groupings withing the cryptocurrency. 

# Techniques Used: 
* StandardScaler() for data normalization
* K Means for clustering 
* PCA for dimensionality reduction
* hvPlot for data visualization

### Steps taken in this challenge:
1. Data Preprocessing:
* loaded cryptocurrency market data into a Pandas DataFrame
* Normalized the Data with StandardScaler() to ensure uniformity

2. Initial Clustering:
* Determined optimal number of clusters (k) using the Elbow Method on scaled data
* Applied K Means clustering with the chose k value
* Visualized clusters using hvPlot.scatter, plottign 24-hour vs 7 day price changes

3. Optimization with PCA:
* Reduced the features to 3 principal components using PCA 
* Re-evaluated optimal k using the Elbow Method on PCA transformed data
* Performed K Means clustering on PCA data
* Visualized PCA data clusters using hvPlot.scatter plot to assess improvement in separation and clarity

4. Analysis:
* Compared clustering results before and after PCA
* Conclusion: Noted enhanced cluster definition and reduced noise with the PCA data
* Both scatter plots showed a general postive correlation. This pattern suggests that short term gains (24-hr price changes) often align with medium term gains (7 day price changes)

# Resources
I used previous class examples for help with my code, along with my tutor Angel Mila. Portions of this ReadMe and explanaitons were enhanced with the assistance of OpenAI's ChatGPT to improve clarity, structure, and understanding of concepts. 

