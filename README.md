# Fully Quantum Image Classification Model

This project explores the implementation of a "fully quantum layer" for image classification and recognition. The construction of convolutional and pooling layers within a quantum circuit follows the proposed QCNN methodology outlined in reference 1. The former layer is designed to capture local correlations, while the latter aims to reduce the dimensionality of the feature vector. In the quantum circuit, the convolutional layer employs a two-qubit unitary, created by sweeping a kernel across the entire image, to correlate neighboring qubits. The pooling layer utilizes a conditioned single-qubit unitary, dependent on the measurement outcome of a neighboring qubit. Lastly, a dense layer is employed to entangle all qubits in the final state using an all-to-all unitary gate, as depicted in the accompanying figure.

## Objective

2023 Ephys Challenge - Quantum Hackathon

## Challenge

Utilize quantum machine learning to classify photos of CIFAR-100.

## Results

For the 8_8_with_zero test set: 0.82 accuracy.

For the 16_16_with_zero test set: 0.84 accuracy.

For the 8_8_with_max test set: 0.86 accuracy.

For the 16_16_with_max test set: 0.91 accuracy.

## File Description

Crawl Data:

> This module includes downloading data from various datasets.

> It transforms the data into (2^n) x (2^n) matrices and extracts the eigenvalues before outputting them.

CIFAR_100_8_8_with_zero.ipynb

> Download the CIFAR-100 dataset and extract classes 3 and 88. Convert the images in these classes to 4x4 matrices, representing three colors, and fill the fourth color with zeros.

CIFAR_100_8_8_with_max.ipynb

> Download the CIFAR-100 dataset and extract classes 3 and 88. Convert the images in these classes to 4x4 matrices, representing three colors, and fill the fourth color with max values.

Train:

> This section encompasses the entire data input, model training, and the recognition of results.

train_8_8.ipynb

> Train the model with 8x8 inputs.

Result

> This section includes information such as training cost, testing cost, training set accuracy, testing set accuracy, and the size of the samples used.

accuracy_8_8 with zero.text

> Using the data downloaded from CIFAR_100_8_8_with_zero, train the model using train_8_8, and obtain the results.

Dataset

> Data captured through web crawling.

CIFAR-100_8_8_with_zero_train.text

CIFAR-100_8_8_with_zero_test.text

## dataset

CIFAR-100 Category 3 and Category 88

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

> Google Colab's operating system is the Ubuntu distribution of Linux

## Author

National Chengchi University, Graduate Institute of Economics, First-year Master's student, Ding-Dang Yang.

Graduated with a Bachelor's degree in Economics from National Cheng Kung University.

## License

This project is free and open source.

## References

1. https://pennylane.ai/qml/demos/tutorial_learning_few_data/

2. McClean, J. R., Boixo, S., Smelyanskiy, V. N., Babbush, R., & Neven, H. (2018). Barren plateaus in quantum neural network training landscapes. Nature communications, 9(1), 4812.

