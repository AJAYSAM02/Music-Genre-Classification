# Music-Genre-Classification
Dataset- The GTZAN genre collection dataset. Each track is in .wav format. It contains audio files of the following 10 genres.
dataset download link: http://opihi.cs.uvic.ca/sound/genres.tar.gz

ABOUT THE PROJECT-
There are many methods present to perform classification on this dataset. We will be using the KNN(K-nearest neighbors) algorithm.
KNN is a supervised machine learning algorithm which works by finding the distances between a query and all the examples in the data, selecting the specified number examples (K) closest to the query, then votes for the most frequent label or averages the labels.
KNN can be used both for classification as well as regression.
KNN algorithm at the training phase just stores the dataset and when it gets new data, then it classifies that data into a category that is much similar to the new data.

- we will first extract features and components from the audio files.
- we will then identify the linguistic content
- then remove noise
- we divide the audio signals into smaller frames, then we try to identify different frequencies present in each frame. Then  separate linguistic frequencies from the noise.
- To discard the noise we take the DCT(discrete cosine transform) of these frequencies. Using DCT we keep only a specific sequence of frequencies that have a high probability of information.

Procedure-
1. import the necessary libraries
2. we define a function to get the distance between feature vectors and find neighbors
3. identifying the nearest neighbors
4. define a function for model evaluation
5. extracting the features from the dataset and dump these features into a binary .dat file [my.dat]
6. train and test split on the dataset
7. make prediction using KNN
8. checking the accuracy of the model on test data

Therefore, we have developed a classifier on audio files to predict its genre.

