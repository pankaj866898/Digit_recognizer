# Digit Recognizer

This project is a digit recognizer built using a Convolutional Neural Network (CNN) with TensorFlow and Keras. The model is trained on the MNIST dataset, which contains images of handwritten digits (0-9).

## Requirements

Make sure you have the following installed:
- Python 3.6+
- TensorFlow 2.x
- NumPy

You can install the required packages using pip:

```sh
pip install tensorflow numpy
```

## Dataset
The MNIST dataset will be automatically downloaded and loaded when you run the code. It is a collection of 28x28 grayscale images of handwritten digits, with a training set of 60,000 examples and a test set of 10,000 examples.

## Model Architecture
The model is a CNN with the following layers:

Convolutional layer with 32 filters and 3x3 kernel size, ReLU activation
MaxPooling layer with 2x2 pool size
Convolutional layer with 64 filters and 3x3 kernel size, ReLU activation
MaxPooling layer with 2x2 pool size
Flatten layer
Dense layer with 128 units, ReLU activation
Dense output layer with 10 units (one for each digit), softmax activation
Training
The model is trained for 10 epochs with a batch size of 200. The Adam optimizer is used with categorical cross-entropy loss and accuracy as the evaluation metric.
