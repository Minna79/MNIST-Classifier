# Fashion MNIST Classifier

A machine learning project for classifying **Fashion MNIST** images using a **K-Nearest Neighbors (KNN)** classifier implemented from scratch.

## Overview

The project uses the Fashion MNIST dataset, which contains 70,000 grayscale 28×28 images from 10 clothing categories.

The workflow includes:

* Exploring and visualizing the dataset
* Splitting the data into training, validation, and test sets
* Min-Max normalization
* Dimensionality reduction using PCA
* 3D visualization using t-SNE
* Implementing KNN from scratch
* Distance-weighted voting
* Hyperparameter tuning
* Evaluating the final model using classification metrics

## Dataset

The Fashion MNIST dataset contains 10 classes:

* T-shirt/top
* Trouser
* Pullover
* Dress
* Coat
* Sandal
* Shirt
* Sneaker
* Bag
* Ankle boot

Each image is represented by its pixel values.

## Method

The dataset is divided into:

* **70% Training**
* **15% Validation**
* **15% Testing**

The preprocessing pipeline applies Min-Max scaling using statistics calculated from the training set, followed by PCA to reduce dimensionality while preserving a specified percentage of variance.

The KNN classifier is implemented without using a pre-built KNN implementation. It calculates Euclidean distances, selects the nearest neighbors, and uses distance-weighted voting for prediction.

## Evaluation

The final model is evaluated on the test set using:

* Accuracy
* Precision
* Recall
* F1 Score
* AUC
* Confusion Matrix
* ROC Curves
* Macro Precision
* Macro Recall
* Macro F1
* Macro AUC

## Technologies

* Python
* NumPy
* Pandas
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook
