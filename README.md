# MIning_master
Machine Learning Project - Unsupersived text aggregation

Any text data be it customer reviews, news articles, social-media data or conversations between people, when we are focused to extract useful insights from them, it is impossible to manually read and summarise them. There are no labels directing this process, hence it is completely unsupervised. Clustering is the ultimate rescue plan when it comes to unstructured data.

For this project, I have taken an interesting problem, to structure the Times of India news articles headlines from Jan2020-Dec2020.

# Data Gathering
The data is scraped from Times of India website https://timesofindia.indiatimes.com/archive/year-2020,month-1.cms archived page. 

# Data Cleaning
As the data we have is news headlines it is pretty clean, just applied the simple logic for tidying it. 

# Data Transformation
Bag of words(BoW) and Term Frequency-Inverse Document Frequency(TF-IDF) uses the frequency of words distribution in the documents, to capture the syntactic importance of the data. Pre-trained sentence transformer model is used to capture semantic understanding of data. All these 3 vectorisation methods are combined together to get the text vectors.

# Data Modelling
K-Means clustering, a simple centroid based clustering algorithm, that aims to partition n observations into k clusters in which each observation belongs to the cluster with the nearest mean, serving as a prototype of the cluster. Introduced a custom idea of bringing hierarchy into k-means based on silhouette scores to identify different domains and sub-domains in the news. Built a tree structure as a result of this process.

# Theme Identification
Used YAKE and TextRank algorithms for extracting the kewords from the clusters identified. 

This standalone idea of bringing hierarchy into k-means based on silhouette scores and keyword extraction on top of that can be used individually to any text data. 
The entire project flow with intution is explained briefly in the medium blog - https://keerthana-ceg.medium.com/text-clustering-the-beginning-f7e787625d49
