# Deep Learning Model for Fashion MNIST

## Overview
This repository contains Jupyter notebooks for training a deep learning model using **TensorFlow** on the **Fashion MNIST** dataset. The models classify images into 10 different categories of clothing. The training process is logged using **Google Cloud Logging**.

## Files

### 1. `updated_model.ipynb`
- Loads the **Fashion MNIST** dataset using `tensorflow_datasets`.
- Preprocesses data: batching without explicit normalization.
- Defines a **Sequential** model:
  - `Flatten` layer to convert 28x28 images into 1D vectors.
  - `Dense(64, activation='relu')` for feature extraction.
  - `Dense(10, activation='softmax')` for classification.
- Trains for **5 epochs** and logs the results to Google Cloud Logging.

### 2. `model.ipynb`
- Similar to `updated_model.ipynb`, but includes explicit **normalization** of input images (`/255.0`).
- Evaluates the model on test data and logs accuracy.
- Uses Google Cloud Logging to track training and evaluation.

### 3. `callback_model.ipynb`
- Implements a **custom callback**:
  - Training stops automatically when accuracy exceeds **84%**.
- Uses the same **Sequential** model structure as the other notebooks.
- Logging is integrated for training progress tracking.

## Requirements
- Python 3.x
- TensorFlow
- TensorFlow Datasets
- Google Cloud Logging (`google.cloud.logging`)

## Usage
1. Install dependencies:
   ```bash
   pip install tensorflow tensorflow-datasets google-cloud-logging
   ```
2. Open and run the notebooks in Jupyter Notebook or Google Colab.
3. Modify parameters (epochs, batch size) as needed.

## Future Improvements
- Experiment with **CNNs** instead of a simple dense network.
- Add **data augmentation** to improve model generalization.
- Optimize **hyperparameters** using Keras Tuner or Grid Search.

## Acknowledgments
- Dataset: [Fashion MNIST](https://www.tensorflow.org/datasets/catalog/fashion_mnist)

