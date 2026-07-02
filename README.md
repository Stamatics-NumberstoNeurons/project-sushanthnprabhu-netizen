# Iris Species Classification Using Neural Network

## Author

Sushanth N Prabhu

## Project Overview

This project implements a complete neural network from scratch using only NumPy and Matplotlib for classification of iris flower species. The objective is to classify flowers into one of the following three categories:

* Iris-setosa
* Iris-versicolor
* Iris-virginica

The model takes four physical flower measurements as input and predicts the corresponding species.

---

## Dataset

The project uses the classic Iris dataset containing 150 samples.

Each sample consists of four numerical features:

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

Output classes:

* Iris-setosa
* Iris-versicolor
* Iris-virginica

Dataset Split:

* Training Set: 120 samples (80%)
* Testing Set: 30 samples (20%)

---

## Data Preprocessing

The following preprocessing steps were performed before training:

1. Loaded the dataset using Python file handling
2. Separated feature values and labels
3. Converted species labels into one-hot encoded vectors
4. Applied Min-Max normalization to scale features between 0 and 1
5. Shuffled the dataset randomly
6. Split data into training and testing sets

---

## Neural Network Architecture

A fully connected feedforward neural network was implemented with the following architecture:

Input Layer:

* 4 neurons

Hidden Layer 1:

* 10 neurons
* Activation Function: ReLU

Hidden Layer 2:

* 5 neurons
* Activation Function: ReLU

Output Layer:

* 3 neurons
* Activation Function: Softmax

Architecture Representation:

4 → 10 → 5 → 3

---

## Mathematical Components

### Activation Functions

* ReLU
* Softmax

### Loss Function

* Cross Entropy Loss

### Optimization Method

* Gradient Descent

### Learning Approach

The model learns using:

* Forward Propagation
* Loss Computation
* Backpropagation
* Weight Updates

---

## Hyperparameters

Learning Rate:
0.01

Epochs:
1000

---

## Libraries Used

Only the following libraries were used:

* NumPy
* Matplotlib

No machine learning frameworks such as TensorFlow, PyTorch, or Scikit-learn were used.

---

## Training Process

During training, the following steps were repeated for each sample:

1. Forward pass through the network
2. Compute prediction probabilities
3. Calculate loss using cross entropy
4. Perform backpropagation
5. Update weights and biases using gradient descent

This process was repeated for 1000 epochs.

---

## Results

The model successfully learned to classify iris flower species with high accuracy.

Training loss decreased significantly over time, indicating effective learning.

Sample loss progression:

Epoch 0: 152.97
Epoch 100: Loss decreased significantly
Epoch 500: Loss continued reducing
Epoch 1000: Final trained model

Final Test Accuracy:
Approximately 90% – 96%

---

## Key Learnings

This project provided practical understanding of:

* Neural Network Architecture
* Forward Propagation
* Backpropagation
* Gradient Descent
* Loss Optimization
* Classification using Deep Learning

It helped build strong intuition about how neural networks learn from data mathematically.

---

## Repository Contents

* Iris_prediction_NN.ipynb
* Iris.csv
* README.md

---

## Conclusion

This project successfully demonstrates the implementation of a neural network from scratch using NumPy for multiclass classification.

The model achieved strong performance on the Iris dataset and provided a practical understanding of the mathematical foundations behind neural networks.
