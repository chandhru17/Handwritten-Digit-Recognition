# Handwritten Digit Recognition using Neural Network

## Introduction

This project focuses on developing a Neural Network model to recognize handwritten digits (0-9) from input images. The model is built from scratch using NumPy for matrix operations and Matplotlib for visualizations. The training data is derived from the MNIST dataset, consisting of grayscale images of handwritten digits.

## Dataset

- **Training Data:** 1000 samples, each represented by a 784-dimensional vector (28x28 images flattened) with corresponding one-hot encoded labels.
- **Test Data:** 350 samples, similarly represented.

## Model Architecture

The Neural Network model consists of the following components:

- **Input Layer:** 784 neurons (28x28 pixel images flattened into a vector)
- **Hidden Layer:** 1000 neurons with Tanh activation function
- **Output Layer:** 10 neurons (one for each digit 0-9) with Softmax activation function

## Activation Functions

The following activation functions and their derivatives are used:

- **Tanh:** Hyperbolic tangent function for the hidden layer.
- **Softmax:** Function for the output layer to convert logits to probabilities.

## Parameter Initialization

Parameters (weights and biases) are initialized randomly for the network layers at first.

## Training the Model

The model is trained using forward propagation, cost computation, backward propagation, and parameter updates. The cost function used is the cross-entropy loss. The training process is iterative, updating the model parameters to minimize the cost.

## Cost vs. Iterations

The cost is monitored over a specified number of iterations to ensure the model is learning appropriately and the cost typically decreases as the number of iterations increases.

## Model Accuracy

The accuracy of the model is evaluated on both the training and test datasets. The accuracy is computed by comparing the predicted labels with the true labels and the result is as follows:

- **Accuracy on Training Dataset:** 95.3%
- **Accuracy on Test Dataset:** 84.57%

## Conclusion

This project demonstrates the implementation of a basic Neural Network for handwritten digit recognition. The model achieved high accuracy on both training and test datasets, illustrating the effectiveness of neural networks for image classification tasks.
