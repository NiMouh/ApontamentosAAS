# Anomaly Detection
Anomaly detection is the identification of abdnormal data points within a dataset.

Anomaalies can be broadly categorized as:

- Point anomalies: A single instance of data is anomalous if it's too far off from the rest. Business use case: Detecting credit card fraud based on "amount spent."
- Contextual anomalies: The abnormality is context specific. This type of anomaly is common in time-series data. Business use case: Spending $100 on food every day during the holiday season is normal, but may be odd otherwise.
- Collective anomalies: A set of data instances collectively helps in detecting anomalies. Business use case: Someone is trying to copy data form a remote machine to a local host unexpectedly, an anomaly that would be flagged as a potential cyber attack.

## Unsupervised Learning
Unsupervised learning is where you only have input data (X) and no corresponding output variables (no labeled data).

## Clustering
The task of dividing the population or data points into a number of groups such that data points in the same groups are more similar to other data points in the same group than those in other groups.

Clustering algorithms:
- K-Means
- Gaussian Mixture Models
- DBSCAN
- Hierarchical Clustering

## Density-Based Anomaly Detection
Density-Based Anomaly Detection is based on the k-nearest neighbors algorithm. It is a non-parametric method for detecting the presence of outliers in a given dataset.

## SVM (Support Vector Machine)
A support vector machine is another effective technique for detecting anomalies. A SVM is typically associated with supervised learning, but there are extensions (OneClassCVM, for instance) that can be used to identify anomalies as an unsupervised problems.

## Isolation Forest Algorithm
The algorithm is based on the fact that anomalies are data points that are few and different. As a result of these properties, anomalies are susceptible to a mechanism called isolation.

## Autoencoders
An autoencoder is a type of artificial neural network used to learn efficient data codings in an unsupervised manner.

It's composed of two parts:
- Encoder: The encoder part of an autoencoder transforms the input data into a compressed representation.
- Bottleneck: The compressed representation of the input data.
- Decoder: The decoder part of an autoencoder transforms the compressed representation into the reconstructed data.

## Confusion Matrix
A confusion matrix is a table that is often used to describe the performance of a classification model (or "classifier") on a set of test data for which the true values are known.

It's a 2x2 matrix:
- True Positive: The number of correct predictions that the occurrence is positive.
- True Negative: The number of correct predictions that the occurrence is negative.
- False Positive: The number of incorrect predictions that the occurrence is positive.
- False Negative: The number of incorrect predictions that the occurrence is negative.

From the confusion matrix, we can calculate:
- the accuracy (TP+TN/TP+TN+FP+FN)
- precision (TP/TP+FP)
- recall (TP/TP+FN)
- F1 score (2*precision*recall/precision+recall).

## Recall vs Precision
- Recall: Out of all the positive classes, how much we predicted correctly. It should be high as possible.
- Precision: Out of all the positive classes we have predicted correctly, how many are actually positive. It should be high as possible.