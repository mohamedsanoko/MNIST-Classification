# MNIST Digit Classification with TensorFlow2

This project demonstrates how to train a neural network model to classify handwritten digits from the MNIST dataset using TensorFlow.

## Data

The MNIST dataset is loaded using TensorFlow Datasets (TFDS). It consists of 60,000 training examples and 10,000 test examples of handwritten digits from 0 to 9. 
10% of the training dataset is used a validation set to prevent overfitting the parameters.

## Model

The neural network model consists of an input layer, three hidden layers with ReLU activation, and an output layer with softmax activation.

- Input layer: 28x28x1 (image dimensions), the input layer is flatten to a 784x1 vector
- Hidden layer sizes: 200 neurons
- Output layer: 10 neurons (one for each digit)

## Training

The model is trained using the Adam optimizer and sparse categorical crossentropy loss function. Training is conducted for 5 epochs with a batch size of 100.

## Results

After training, the model achieves an accuracy of approximately 98.85% on the validation set and 97.99% on the test set.

## Requirements

- Python 3
- TensorFlow2
- TensorFlow Datasets (tfds)
