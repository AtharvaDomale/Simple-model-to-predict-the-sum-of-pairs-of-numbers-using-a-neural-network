# Predicting the Sum of Pairs of Numbers

## Project Overview

This project demonstrates how to create a simple neural network model using PyTorch to predict the sum of pairs of numbers. The model is trained on a dataset consisting of pairs of numbers and their corresponding sums, showcasing the fundamental components of a training loop in PyTorch.

## Dataset

The dataset is generated from a specified range of numbers (e.g., 1 to 100). For each combination of two numbers, the target output is the sum of those two numbers. The dataset contains all possible pairs, resulting in \( n^2 \) pairs for \( n \) numbers.

### Example Data Points

- Input: (1, 1) → Output: 2
- Input: (3, 7) → Output: 10
- Input: (5, 5) → Output: 10

## Model Architecture

The model consists of the following layers:

- **Input Layer**: Accepts two input features (the two numbers).
- **Hidden Layer**: A single hidden layer with 128 neurons, using the ReLU (Rectified Linear Unit) activation function.
- **Output Layer**: A single neuron that predicts the sum of the input numbers.

## Training Process

The model is trained using the following components:

- **Loss Function**: Mean Squared Error (MSE) is used to measure the difference between predicted sums and actual sums.
- **Optimizer**: Adam optimizer is utilized to update the model's parameters based on the computed gradients during backpropagation.
- **Training Loop**: The training loop iterates through multiple epochs, processing the dataset in batches to minimize the loss.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/predict-sum-of-pairs.git
   cd predict-sum-of-pairs
