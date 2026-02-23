# Neural Network Pattern Recognition: Handwritten Digit Classification

## Project Overview
This project implements a supervised learning system to classify digits (0-9) from the Scikit-learn digits dataset. The project includes:
1. **Neural Architecture Study**: Analyzing how hidden layer complexity (neuron count) impacts classification accuracy.
2. **High-Dimensional Visualization**: Using four distinct unsupervised learning methods to map 64-dimensional pixel data into a 2D plane.

## Technical Implementation
### 1. Supervised Learning (MLP)
* **Model**: Multi-Layer Perceptron (ANN).
* **Optimization**: Stochastic Gradient Descent (SGD) with Sigmoid activation.
* **Results**: Achieved an average accuracy of **~92.6%** through an optimization loop testing 30 different hidden layer architectures (5-34 neurons).

### 2. Dimensionality Reduction & Visualization
To understand the mathematical "separability" of the data, I compared four different techniques:
* **PCA (Linear)**: Capturing maximum variance.
* **t-SNE (Probabilistic)**: High-fidelity clustering of similar digits.
* **Isomap (Manifold)**: Preserving the "geodesic" distance along curved data structures.
* **Spectral Embedding (Graph Theory)**: Mapping data based on connectivity.

## Key Findings
* **Complexity vs. Accuracy**: Increasing the hidden layer size from 5 to 34 neurons showed a clear trend in stabilizing model performance.
* **Clustering**: t-SNE provided the most distinct separation, suggesting that digit recognition is highly dependent on local neighborhood relationships in the pixel space.

## Environment & Libraries
* **Language**: Python 3.x
* **Libraries**: NumPy, Matplotlib, Scikit-learn
* **Editor**: Visual Studio Code (Jupyter Extension)

