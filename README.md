# Neural Network from Scratch (NumPy Implementation)

## Project Overview and Purpose
This project is an educational implementation of a Multi-Layer Perceptron (MLP) built entirely from scratch using Python and NumPy. By manually coding the mathematical foundations of neural networks—including activation functions, forward passes, and gradient-based backpropagation—this repository serves as a deep dive into how neural networks learn and optimize parameters for complex tasks.

## Key Technologies and Libraries
- **Mathematics & Logic**: `NumPy`
- **Data Preprocessing**: `scikit-learn` (StandardScaler, train_test_split)
- **Synthetic Data**: `scikit-learn` (make_regression)
- **Environment**: Python 3 / Jupyter Notebook

## Technical Implementation
### 1. Model Architecture
The network is designed as a flexible class structure that supports:
- [cite_start]**Input Layer**: Configurable based on input feature dimensions[cite: 1].
- [cite_start]**Hidden Layer**: Configurable number of neurons (e.g., 128) with **ReLU** activation[cite: 1, 3, 6].
- [cite_start]**Output Layer**: Supports both **Linear** activation (for regression) and **Sigmoid** activation (for classification)[cite: 1].

### 2. Core Functions
- [cite_start]**Forward Propagation**: Calculated as $A = \text{activation}(W \cdot X + b)$[cite: 3].
- [cite_start]**Error Metrics**: Implemented Mean Squared Error (**MSE**) for regression and **Cross-Entropy** for classification tasks[cite: 3, 4].
- [cite_start]**Backpropagation**: Manually calculated gradients for weights and biases using the chain rule to update the network's parameters over time[cite: 4, 5].


## Results and Insights
- [cite_start]**Optimization**: Tested on a synthetic regression dataset with 1,000 samples and 3 features[cite: 5].
- [cite_start]**Training Performance**: The model demonstrated successful convergence, reducing the loss from **13,892.78** at epoch 0 to **350.32** by epoch 4,500.
- [cite_start]**Weight Initialization**: Utilized random normal distributions for weights and biases to ensure varied feature learning from the start[cite: 1].

## How to Run
1. Install the minimal dependencies:
   ```bash
   pip install -r requirements.txt
