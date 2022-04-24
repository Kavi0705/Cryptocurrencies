# Cryptocurrencies

## Purpose
The purspose of this analysis is to use unsupervised machine learning techniques in order to determine the different types of cryptocurrencies that exist on the trading market, and group them to create a classification system to create a new cryptocurrency investment portfolio.

## Results

First, the data had to be preprocessed and transformed. This included dropping null values, using only tradable and mined cryptocurrencies, numerically encoding categorical columns using the get_dummies() method, and scaling the data using the StandardScaler() method as well.

Then, the Principal Component Analysis (PCA) was completed in order to reduce the 98 scaled columns to only 3 principal components.

<img width="254" alt="PCA" src="https://user-images.githubusercontent.com/93743169/164999458-13410100-38cf-4925-8f70-acbad4cf381c.png">

Thirdly, using the hvPlot method an elbow curve was created to find the best value for K. From there, teh K-means algorithm was used to predict the K clusters for the cryptocurrenceis' data.

<img width="785" alt="Elbow curve" src="https://user-images.githubusercontent.com/93743169/164999585-f0dfdaed-ab88-4e1b-9191-89619bfa6dda.png">

As one can see, the best k value appears to be 4 so it would be recommended on an output of 4 clusters to categorize the crytocurrencies. 

Finally, a 3-D scatter plot was generated to plot the 3 clusters.

<img width="844" alt="3D Scatter Plot" src="https://user-images.githubusercontent.com/93743169/164999854-18286ec1-4aec-4973-9a63-f25e492faec2.png">

A 2-D scatter plot was also generated to visualize the 3 clusters to 2 principal components.

<img width="702" alt="hv 2-d scatter plot" src="https://user-images.githubusercontent.com/93743169/164999998-8cf7dd2a-cd68-402e-b775-5eb26354cdb6.png">

<img width="723" alt="Tradable cryptocurrencies table" src="https://user-images.githubusercontent.com/93743169/164999962-e6d21a10-d073-410d-b269-f96e92527e90.png">

Following the preprocessing and cleaning phase we have a total of 532 tradable cryptocurrencies. Most of the cryptocurrencies are part of class #0 and #1.

## Summary

A classification of 532 cryptocurrencies based on similarities of their features were identified from all the data. Most fall into 2 classes. However, particularities of each group need to be analyzed to determined their performance and potential to be included in an investment portfolio.
