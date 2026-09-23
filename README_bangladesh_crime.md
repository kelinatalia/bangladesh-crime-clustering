# Bangladesh Crime Clustering

## Overview
This project groups districts in Bangladesh based on crime and demographic patterns using K-Means clustering. The dataset has 6,574 rows and 26 columns, covering crime records, weather, population, and infrastructure data.

## Steps
- Data cleaning: replaced placeholder values with missing values, imputed missing data, fixed inconsistent weekday labels, handled outliers by capping
- Exploratory data analysis: looked at crime type distribution, crime by season, crime by time of day, and the relationship between population and police stations
- Encoding and scaling: label encoding for categorical columns, RobustScaler for numeric columns
- Clustering: used the elbow method and silhouette score to find the best number of clusters, then applied K-Means
- Visualization: used PCA to plot the clusters in 2D
- Profiling: labeled each cluster based on its characteristics (for example, high population and high crime, or low population and low crime)

## Result
The districts are grouped into 3 clusters with different risk levels, based on population density, infrastructure, and crime rate. Dhaka stands out as a high risk cluster because of its very high population density.

## Files
```
No_2.ipynb                          # Main notebook
Bangladesh_Crime_Dataset_B.csv      # Dataset
```

## Tech Stack
Python, pandas, numpy, scikit-learn, seaborn, matplotlib
