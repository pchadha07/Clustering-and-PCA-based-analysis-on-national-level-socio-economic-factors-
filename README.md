# Clustering-and-PCA-based-analysis-on-national-level-socio-economic-factors-
The requirement of this assignment, “Clustering of Countries”, is to shortlist countries that are 
in immediate need of financial aid. I did this by creating clusters (both using Hierarchical and Kmeans clustering) based on top five Principal components calculated using PCA algorithm/functions. 
The five principal components were linear transformations of given socio-economic defining 
parameters, such as ‘GDP per capita’, ‘income’, ‘child_mort’, ‘total_fer’, ‘imports’, ‘exports’, etc, in 
the dataset for list of 167 countries. Following are the steps that were carried out to derive the final 
list of countries:
• Perform EDA to check for missing values, duplicate entries, outlier analysis and format 
conversion to make sure that data is free from any irregularities
• Scale the numeric data using Standard scaler so that all the numeric variables, which in this 
case are all the relevant independent variables, are within specific range. Scaling also is one 
of the main requirements for PCA to produce accurate results
• Perform PCA to identify the top principal components that explain maximum variance and 
hence, help in dimensionality reduction
• I selected five principal components as they explained in total of approximately 96% 
variance 
• Next, performed ‘Hopkins’ test to verify whether the dataset (5 PCs) was applicable for 
clustering. A high score of above 80% was achieved and so proceeded with clustering
• First performed K-means clustering. First step involved identifying the optimum number of 
clusters via ‘elbow-curve’ and ‘silhouette score’ analysis. Both revealed the ideal number of 
clusters to be ‘3’ and so proceeded with creating K-means cluster model with ‘3’ clusters
• Three distinct clusters were achieved and cluster - ‘0’ was identified to be the one consisting 
of countries that have poorest of socio-economic conditions and so was selected for further 
analysis to shortlist the countries. This was possible with the help of ‘boxplots’
• ‘Means’ of ‘child-mort’, ‘income’, ‘gdpp’ and even ‘total-fer’ were used to further shortlist 
the countries and the final list consisting of six countries was derived that need financial aid 
the most and on immediate basis.
• Clustering was then performed on the same five ‘PCs’ as above, using both ‘single’ and 
‘complete’ linkage
• The ‘complete’ linkage revealed the ideal number of clusters to be ‘3’, same as in the case of 
K-means clustering
• Cluster- ‘0’ was even in this case identified with countries that required the aid most 
immediately based on box-plot analysis. Though the size of this cluster in this case was 
almost half when compared to the same cluster formed in K-means analysis• Similar steps were performed to filter the countries further as were carried out in K-Means 
clustering and the final list of countries came out to be the same as in the case of K-means 
clustering
