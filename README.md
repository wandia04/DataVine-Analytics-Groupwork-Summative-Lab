# DataVine-Analytics-Groupwork-Summative-Lab
We went through the summative lab so as to divide the work amongst ourselves. Everyone downloaded the dataset they were working on; the Wine, Chickwts and USArrests datasets
We first understood what the datasets were talking about, prepared the data by checking if there were any missing values, duplicate values and any inconsistencies. We then cleaned the data and standardized the numerical features using StandardScaler for the ones required

For Chickwts recommendation system, we used PCA to reduce the dimensionality to one (PC1) which showed the standardized weight between the feed types
We then applied cosine similarity to see which feed types had the similar PC1 values. Casein, meatmeal and sunflower had positive similar relationships while horsebean, linseed and soybean had negative similar relationships.
When we look at the cosine similarity results, casein can be recommended as similar to meatmeal and sunflower, while horsebean can be similar to linseed and soybean based on the weight feature.
In conclusion, we cannot say one is the best alternative to the other because we are only checking similarity based on the feed weight

For USArrests clustering, it was first standardized and reduced using PCA before doing K-means and Gaussian Mixture Models (GMM). The PCA retained 86.75% of the total variance, this allowed most of the important information to remain and be represented in the two dimensions
K-means clustering was used with 4 clusters and produced a silhouette score of 0.444 and GMM selected 2 clusters based on the lowest Bayesian Information Criterion(BIC).
After using the two methods, we saw it gave different groupings of states because K-means groups based on distance from cluster centers, while GMM uses a probabilistic approach
In conclusion,clustering results show that states can be grouped according to similarities in their crime measurements and these clusters can help identify patterns in crime data and provide groups of states that can be explored further.

For the Wine dataset, we built a supervised k-Nearest Neighbors (k-NN) classifier optimized with Principal Component Analysis (PCA) and cross-validated grid search:  
Dimensionality Reduction (PCA): Reduced features from 13 dimensions down to 10 principal components while preserving >95% cumulative variance.  
Hyperparameter Optimization (GridSearchCV): Used 5-fold cross-validation to search for optimal values across k \in [1, 20], distance metrics (p=1 Manhattan, p=2 Euclidean), and weighting schemes (uniform, distance).  
Best Configuration: KNeighborsClassifier(n_neighbors=13, p=1, weights='uniform').  
Performance: Achieved a 5-fold cross-validation accuracy of 97.72% and a final held-out test set accuracy of 97.78%.

Our group members are Faith, Hafsa ,Wandia, Yefta and Alvin. And we divided the work as follows Yefta and Alvin worked on K-NN classification on the wine dataset, Wandia worked on building a recommendation system using Chickwts dataset and Hafsa and Faith worked on clustering using K-means and GMM using the USArrest dataset. We met online and discussed the work as we did it in the notebook, then decided who was to push the notebook here, instead of sending the same notebook twice
