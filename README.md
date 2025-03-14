# Unsupervised-ML-Moosic

Unsupervised ML Case study: Moosic

Moosic, a small emerging company, specializes in crafting playlists meticulously curated by music experts with a keen eye on both classic and contemporary trends. With a dataset comprising approx. 5000 songs, encompassing details on distinct audio attributes like tempo, energy, and danceability, Moosic has tasked us with employing advanced clustering algorithms such as K-Means. The objective is to categorize the dataset into several clusters, creating recommendations for users with diverse playlists.

With this, we should be able to answer the following two questions:

    Are Spotify’s audio features able to identify “similar songs”, as defined by humanly detectable criteria?
    Is K-Means a good method to create playlists?

As a deliverable, we will present our findings to Moosic CEO.
Data Cleaning and Scaling

We first clean our data by dropping missing values and duplicates. For columns containing strings (song and artist names), we omit redundant spaces. We then scale data using MinMaxScaler().
Layered Approach to Clustering

We perform clustering by following a layered approach described below.
Main Clusters

To obtain our main clusters, we first identify relevant features using the Principal Component Analysis (PCA). We then select the number of main clusters using the Elbow and Silhouette charts (5 clusters).
Subclusters

We repeat the above procedure to create 5 subclusters for each of our main clusters. In total, we obtained 25 subclusters that we analyzed.

The presentation slides discuss the efficacy of these subclusters and provide our take on the questions asked (see presentation slides).

