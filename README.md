# DataVine-Analytics-Groupwork-Summative-Lab
We went through the summative lab so as to divide the work amongst ourselves. Everyone downloaded the dataset they were working on; the Wine, Chickwts and USArrests datasets
We first understood what the datasets were talking about, prepared the data by checking if there were any missing values, duplicate values and any inconsistencies. We then clenaed the data and standardized the numerical features using StandardScaler for the ones required

For Chickwts recommendation system, we used PCA to reduce the dimensionality to one (PC1) which showed the standardized weight between the feed types
We then used cosine similarity to see which feed types had the similar PC1 values. Casein, meatmeal and sunflower had positive similar relationships while horsebean, linseed and soybean had negative similar relationships.
When we look at the cosine similarity results, casein can be recommended as similar to meatmeal and sunflower, while horsebean can be similar to linseed and soybean based on the weight feature 
In conclusion, we cannot say one is the best alternative to the other because we are only checking similarity based on the feed weight

For USArrests clustering, it was first standardized and reduced using PCA before doing K-means and GMM. The PCA retained 86.75% of the total variance, this allowed most of the important information to remain and be represented in the two dimensions
K-means clustering was used with 4 clusters and produced a silhouette score of 0.444 and GMM selected 2 clusters based on the lowest BIC
After using the two methods, we saw it gave different groupings of states because K-means groups based on distance from cluster centers, while GMM uses a probabilistic approach
In conclusion,clustering results show that states can be grouped according to similarities in their crime measurements and these clusters can help identify patterns in crime data and provide groups of states that can be explored further 

Our group members are Faith, Hafsa ,Wandia, Yefta and Alvin. And we divided the work as follows Yefta and Faith worked on K-NN classification on the wine dataset, Wandia worked on building a recommendation system using Chickwts dataset and Hafsa and Alvin worked on clustering using K-means and GMM using the USArrest dataset. We met online and discussed the work as we did it in the notebook, then decided who was to push the notebook here, instead of sending the same notebook twice
