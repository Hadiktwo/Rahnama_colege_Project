# k-Nearest Neighbors from Scratch on Wine Dataset

This project implements the k-Nearest Neighbors (kNN) classification algorithm from scratch using only NumPy. The goal is to classify wines into one of three classes based on 13 chemical features from the Wine dataset.

The dataset is loaded from `sklearn.datasets.load_wine`, but the kNN algorithm itself is implemented manually without using `sklearn.neighbors.KNeighborsClassifier`.

## Project Overview

In this project, I:

- Loaded and explored the Wine dataset
- Split the data into training and test sets
- Standardized the feature values to make distance calculations fair
- Implemented Euclidean distance from scratch
- Found the `k` nearest training samples for each test sample
- Predicted the class using majority voting
- Tested different values of `k`
- Reported the accuracy for each value of `k`

## Dataset

The Wine dataset contains:

- 178 total wine samples
- 13 numerical chemical features
- 3 target classes: `0`, `1`, and `2`

Each row represents one wine sample, and the target label represents its wine class.

## Method

The kNN algorithm works by comparing a new wine sample with the training samples. It calculates the distance between the new sample and every training sample, selects the `k` closest ones, and predicts the class that appears most frequently among those neighbors.

## Technologies Used

- Python
- NumPy
- pandas
- scikit-learn only for loading the dataset and splitting the data
- Matplotlib for optional visualization

## Goal

The main goal of this project is to understand how kNN works internally instead of relying on a ready-made machine learning model.
