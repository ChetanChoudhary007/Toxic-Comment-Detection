# Toxic Comment Detection

![Toxic Comment Detection](https://miro.medium.com/v2/resize:fit:1260/1*l48BVmSlK6o553WxTg3ocw.png)

## Project Overview

This project focuses on developing a toxic comment detection model using deep learning techniques. The model is designed to classify comments as toxic or non-toxic based on a labeled dataset, employing a sequential neural network architecture.

## Table of Contents

1. [Installation](#installation)
2. [Dataset](#dataset)
3. [Preprocessing](#preprocessing)
4. [Data Pipeline](#data-pipeline)
5. [Model Architecture](#model-architecture)
6. [Training](#training)
7. [Evaluation](#evaluation)
8. [Model Prediction](#model-prediction)
9. [Testing with Gradio](#testing-with-gradio)

## Installation

Ensure all required dependencies are installed before running the code:

```bash
pip install tensorflow pandas matplotlib sklearn gradio
```

## Dataset

The training dataset is loaded from a CSV file (`train.csv`) containing comment text and corresponding toxicity labels.

## Preprocessing

Text preprocessing involves tokenizing comments and converting them into a format suitable for deep learning. The `TextVectorization` layer from TensorFlow is used for tokenization.

## Data Pipeline

A robust data pipeline is created using TensorFlow's `Dataset` API, including mapping, caching, shuffling, batching, and prefetching. This pipeline is crucial for efficient training.

## Model Architecture

The deep learning model is a sequential neural network with an embedding layer, bidirectional LSTM layers, and dense layers with activation functions. The model is compiled using the Adam optimizer and binary cross-entropy loss.

## Training

The model is trained on the training dataset for a specified number of epochs, with validation on a separate dataset.

## Evaluation

Model performance is evaluated using precision, recall, and categorical accuracy metrics on a test dataset.

## Model Prediction

The trained model can make predictions on new comments.

## Testing 

The model is tested , allowing users to input comments and observe the model's predictions interactively.
