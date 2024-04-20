# Neuron and Perceptron Implementation

This repository contains Python code implementing a neural network neuron (`Neuron` class) and a Perceptron classifier (`Perceptron` class) using NumPy and other libraries.

## Resources :floppy_disk:

[![Video and Code Materials](https://img.shields.io/badge/📹%20Video%20&%20Code%20Materials-Google%20Derive-blue?style=for-the-badge&logo=google-drive)](https://drive.google.com/drive/folders/1ff8Hm3wIZqrSkmwgh6qEnve6_hBeY-Fc?usp=sharing)

## Neuron Class

The `Neuron` class implements a single neuron model capable of:

- Activation functions: ReLU, Sigmoid, and Hyperbolic Tangent (tanh)
- Loss functions: Binary Cross Entropy (BCE) and Mean Squared Error (MSE)
- Training through gradient descent
- Prediction and evaluation with accuracy

### Methods:

- `__init__(self, in_features, af=None, loss_fn=mse, n_iter=100, eta=0.1, verbose=True)`: Initializes the neuron with parameters.
- `predict(self, x)`: Predicts output given input data.
- `fit(self, x, y)`: Trains the neuron on input `x` and target `y`.
- `gradient(self, x, y, y_hat)`: Calculates gradients for weights and biases.
- `gradient_descent(self)`: Updates weights and biases using gradient descent.
- `parameters(self)`: Returns the neuron's parameters.

### Usage:

Instantiate a `Neuron` object and use `fit` to train the neuron on data `X` and target `y`. Example:

```python
neuron = Neuron(2, af=sigmoid, loss_fn=bce, n_iter=500)
neuron.fit(X, y[:, None])
```

## Neuron Class

The `Neuron` class is a single neuron model featuring:

- Activation functions: ReLU, Sigmoid, and Hyperbolic Tangent (tanh)
- Loss functions: Binary Cross Entropy (BCE) and Mean Squared Error (MSE)
- Training using gradient descent
- Prediction and evaluation, including accuracy calculation

## Perceptron Class

The `Perceptron` class leverages `sklearn.linear_model.Perceptron` for classification tasks. It comprises functionalities for:

- Loading and segregating datasets
- Training the Perceptron classifier
- Accuracy assessment on both training and test sets
