# Deep Neural Network Book Recommender

## Overview

This project aims to create and optimize a book recommender system using a deep neural network. The dataset used contains data for 10,000 books and 53,424 users, sourced from [Goodreads](https://www.kaggle.com/zygmunt/goodbooks-10k).

## Table of Contents

1. [Introduction](#introduction)
2. [Load the Data](#load-the-data)
3. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
4. [Model Preparation, Training, and Optimization](#model-preparation-training-and-optimization)
5. [Conclusion](#conclusion)

## Introduction

This project explores the creation of a book recommender system using TensorFlow and Google Colab. The goal is to predict user ratings for books based on historical data.

## Load the Data

The data is pulled from the Goodreads website. The following datasets are used:
- `books.csv`: Contains information about the books.
- `ratings.csv`: Contains user ratings for the books.
- `to_read.csv`: Contains information about books users want to read.

## Exploratory Data Analysis (EDA)

The EDA section includes:
- Checking the shape and data types of the datasets.
- Describing the datasets to identify any necessary corrections.
- Visualizing the distribution of ratings and the number of ratings per user and book.

## Model Preparation, Training, and Optimization

The model is built using TensorFlow's Keras API. The steps include:
1. **Data Preparation**: Shuffling and splitting the dataset into training and testing sets.
2. **Model Architecture**: Creating input layers for user and book IDs, embedding layers, and dense layers.
3. **Training**: Compiling and training the model with Mean Squared Error (MSE) as the loss function.
4. **Evaluation**: Evaluating the model's performance on the test set.

### Key Components

- **Embeddings**: Used to represent users and books in a lower-dimensional space.
- **Dense Layers**: Used to learn complex interactions between users and books.
- **Callbacks**: TensorBoard for visualization and ModelCheckpoint for saving the best model.

## Conclusion

The project demonstrates the challenges of optimizing a deep learning model for recommendation systems. Despite various attempts, the MSE loss did not improve significantly. Future steps include working with a smaller sample, overfitting, and then regularizing the model, as well as oversampling instances with low ratings.

## How to Run

1. Clone the repository.

2. Install the required packages from requirements.txt.

3. Run the Jupyter notebook in the folder where the Notebook is located.

* NB - please note that the packages in the requirements.txt file are as per the stable version at the time of writing the original project. You may need to update the packages based on the latest versions which might affect the code.
