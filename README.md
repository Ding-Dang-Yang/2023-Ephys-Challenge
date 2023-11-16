# Fully Quantum Image Classification Model

This project involves utilizing a "fully quantum layer" for image classification and recognition. To construct a convolutional and pooling layer in a quantum circuit, we will follow the QCNN construction proposed in 1. The former layer will extract local correlations, while the latter allows reducing the dimensionality of the feature vector. In a quantum circuit, the convolutional layer, consisting of a kernel swept along the entire image, is a two-qubit unitary that correlates neighbouring qubits. As for the pooling layer, we will use a conditioned single-qubit unitary that depends on the measurement of a neighboring qubit. Finally, we use a dense layer that entangles all qubits of the final state using an all-to-all unitary gate as shown in the figure below.

## Objective

2023 Ephys Challenge - Quantum Hackathon

## Challenge

Utilize quantum machine learning to classify photos of xxx.

## dataset

我也還不知道

## Package Usage

pennylane: Quantum computing package used for quantum machine learning and quantum computing.

jax: Package for efficient gradient computation and numerical calculations.

optax: Optimization package based on jax, used for solving optimization problems.

matplotlib: Python library for creating data visualization plots.

numpy: Package for handling and manipulating large numerical arrays and matrices.

pandas: Package providing data structures for data manipulation and analysis.

scikit-learn (sklearn): Package offering machine learning algorithms and tools.

## Development Environment

This model was developed and executed entirely on Colab.

## Author

National Chengchi University, Graduate Institute of Economics, First-year Master's student, Ding-Dang Yang.

## License

This project is free and open source.
