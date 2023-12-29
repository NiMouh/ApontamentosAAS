
# Slide 1 - What is ML (Machine Learning)?
The capability of a machine to improve its own performance.

## Process of Machine Learning
1. Gather Data
2. Clean Data
3. Build Model
4. Gain Insights from the Model results
5. Data Visualization

## Types of Machine Learning
- Supervised Learning: the model is trained with labeled data.
  - Regression;
  - Classification (i.e. KNN, Naive Bayes, SVM);
  - Decision Tree;
  - Random Forest;
- Unsupervised Learning: the model is trained with unlabeled data.
  - Clustering;
  - Association;
  - Hidden Markov Model;
- Reinforcement Learning: the model is trained with rewards and punishments.

Note: the supervised classification can have **discriminative** or **generative** models, however, the unsupervised classification can **only** have generative models.

## Limitations of Machine Learning
When the data is **not enough**, the model will not be able to learn properly. And for every dimension added to the data, the amount of data needed **increases exponentially** (curse of dimensionality).

## Bias vs Variance
- Bias: how far the model is from the real value;
- Variance: how much the model changes when trained with different data.

# Slide 2 - Spam Detection
Spam is an unsolicited email sent to a large number of recipients.

## Process of Spam Detection
1. Binary Classification: spam or not spam;
2. Text Mining: extract features from the text;
   1. NLP (Natural Language Processing): process the text to extract features;
3. Classification Model;
4. Optimization.
5. Feature Selection: select the most relevant features;
6. Model Evaluation: evaluate the model with the test data;
7. Model Deployment: deploy the model to production.

## Bag of Words
A model used to extract features from text. It's a matrix with the number of occurrences of each word in the text.

# Slide 3 - Anomaly Detection

## Signature detection 
Requires knowing what to look for and comparing hashes or other strings to identify a match. Signature detection is a
common feature found within antivirus and IPS/IDS products.

## Behavior detection 
Looks for malicious or other known behavior characteristics and alarms the SOC when a match is made. An example is
identifying port scanning or a file attempting to encrypt your hard drive, which is an indication of ransomware behavior. Antimalware and sandboxes are examples of tools that heavily leverage behavior detection capabilities.

## Anomaly detection 
It takes into consideration hot topics including big data,
threat intelligence, and “zero-day” detection.

# Common reasons for outliers are:
- data preprocessing errors;
- noise;
- fraud;
- attacks

## Types of Anomaly Detection
- Supervised: the model is trained with labeled data;
  - Binary Classification;
  - Multiclass Classification;
- Unsupervised: the model is trained with unlabeled data;
  - Blind Signal Separation;
  - Clustering;

## Blind Signal Separation
The task of recovering a set of source signals from a set of mixed signals, without the aid of information (or with very little information) about the source signals or the mixing process.

**Principal component analysis**, or PCA, is a statistical procedure that allows you to summarize the information content in large data tables by means of a smaller set of “summary indices” that can be more easily visualized and analyzed.

**Independent Component Analysis** (ICA) is a powerful technique in the field of data analysis that allows you to separate and identify the underlying independent sources in a multivariate data set