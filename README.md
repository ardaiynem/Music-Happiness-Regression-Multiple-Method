# Predicting Emotional Valence of Musical Pieces

## Introduction to the Problem

The objective of this project is to predict the emotional valence of musical pieces on a scale ranging from 0 to 1, where 0 represents negative emotions such as melancholy and anger, and 1 represents positive emotions like happiness and joy. Various machine learning regression methods will be employed, including Linear Regression, Ridge Regression, Lasso Regression, Neural Network, and K-Nearest Neighbors Regression. Leveraging the Spotify API Dataset, which contains numerical data on characteristic elements and valence values for thousands of musical pieces, allows for a comprehensive analysis. By employing different algorithms, each with its unique capabilities in capturing underlying patterns, this regression task aims to provide insights into the emotional content of musical compositions.

## Dataset Analysis

The Spotify API provides metrics related to musical characteristics of every piece on Spotify in JSON format. The dataset used for this project, sourced from Kaggle, contains metrics for nearly 100,000 pieces from 125 different genres and is provided in CSV format. The musical characteristic metrics include various features such as duration, danceability, energy, key, loudness, mode, speechiness, acousticness, instrumentalness, liveness, valence, tempo, and time signature. These metrics provide valuable insights into the emotional content of musical pieces. After preprocessing, the dataset has the shape (114000 x 15), with features relevant to our problem.

## Preprocessing

Several preprocessing steps are applied to prepare the dataset for training:
- One-hot Encoding: Convert categorical variables into binary vectors.
- Shuffling: Randomize data instances’ order to prevent sequence-based patterns from influencing learning.
- Standardization (Standard Scaling): Scale features to have a mean of 0 and a standard deviation of 1.
- Normalization (Min-Max Scaling): Scale features to a range between 0 and 1.
- Principal Component Analysis (PCA): Dimensionality reduction technique used to transform high-dimensional data into a lower-dimensional space while preserving most of its variance.

## Used Methodologies and Performance Metrics

The following methodologies are utilized for prediction, and performance metrics are used to evaluate their effectiveness:

### Linear Regression
- Normal Equation
- Pseudo-inverse
- Gradient Descent

### Ridge Regression
- Normal Equation
- Gradient Descent

### Lasso Regression

### Neural Network
- Full Batch with Adam Optimizer
- Full Batch with Stochastic Gradient Descent (SGD)
- Full Batch with Momentum
- Full Batch with RMSProp
- Full Batch with AdaGrad
- Full Batch with Nesterov Momentum
- Full Batch with Adam Optimizer (different network structure)
- Full Batch with AMSGrad
- Full Batch with PCA
- Mini Batch with Adam Optimizer
- Stochastic Gradient Descent with Adam Optimizer

### K-Nearest Neighbors Regression

Please refer to the project "Project_Report.pdf" for detailed results and analysis.
