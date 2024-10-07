# Quantum Neural Network (QNN) with Qiskit

This project demonstrates the implementation of a **Quantum Neural Network (QNN)** using the **Qiskit Machine Learning** library. The notebook implements both **Estimator-based QNN** and **Sampler-based QNN** models for training and inference on quantum circuits.

## Project Overview

Quantum Neural Networks (QNNs) are quantum analogs of classical neural networks. They leverage quantum circuits to perform computations on quantum states and can be used for tasks such as classification, regression, and more. In this project, we construct two types of QNNs:

1. **Estimator QNN**: This QNN computes the expected value of a given observable using a quantum circuit with parameterized gates.
2. **Sampler QNN**: This QNN uses sampling (with a specified number of shots) to estimate the probabilities of certain measurement outcomes, which can be interpreted as the QNN's output.

### Key Components:
- **Quantum Circuit Construction**: Quantum circuits are built with parameterized gates for both input features and learnable weights.
- **Forward and Backward Pass**: The notebook demonstrates how to compute the QNN's output (forward pass) and how to calculate gradients (backward pass), which are essential for training the model.
- **Observable**: A custom observable (Pauli-Y basis) is used to measure the output of the quantum circuit.

## Dependencies

This project requires the following Python libraries:

- `qiskit`: For building quantum circuits, simulating quantum circuits, and defining QNNs.
- `qiskit_machine_learning`: For Quantum Neural Network implementations like `EstimatorQNN` and `SamplerQNN`.
- `numpy`: For handling numerical operations.

You can install the dependencies using:

```bash
pip install qiskit qiskit-machine-learning numpy
