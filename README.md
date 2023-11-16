# Fully Quantum Image Classification Model

This project explores the implementation of a "fully quantum layer" for image classification and recognition. The construction of convolutional and pooling layers within a quantum circuit follows the proposed QCNN methodology outlined in reference 1. The former layer is designed to capture local correlations, while the latter aims to reduce the dimensionality of the feature vector. In the quantum circuit, the convolutional layer employs a two-qubit unitary, created by sweeping a kernel across the entire image, to correlate neighboring qubits. The pooling layer utilizes a conditioned single-qubit unitary, dependent on the measurement outcome of a neighboring qubit. Lastly, a dense layer is employed to entangle all qubits in the final state using an all-to-all unitary gate, as depicted in the accompanying figure.

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

## References

1. https://pennylane.ai/qml/demos/tutorial_learning_few_data/
