# What is this?

This notebook displays the implementation of basic Neural Network using only numpy. The network is trained and tested on the MNIST dataset (loaded with sklearn for ease).

# How to Run

Install the relevant packages with conda or pip.

## Implementation Details

The network is implemented with the following architecture:

- Input Layer: 784 neurons (28x28 pixels)
- Hidden Layers: 128 neurons, 64 neurons, 32 neurons
- Output Layer: 10 neurons (0-9 digits)

The activation functions for each layer are:

- Hidden Layers: ReLU, SELU and tanh
- Output Layer: Softmax

The network is trained with the following hyperparameters:

- Learning Rate: [0.0001, 0.001, 0.01, 0.1]
- Weight Initialization: Xavier, He

The network is trained with the following optimizers:

- Mini-batch SGD, Adam

Loss function: Categorical Cross-entropy (because it's a multi-class classification problem)

# Results

The hyperparameters found to be most effective are learning rate: 0.01 and weight initialization: He. The network was trained with the Adam optimizer and achieved an accuracy of 97.56% on the test set.
