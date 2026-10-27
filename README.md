# Machine Learning: Optimization and Initialization

This repository contains two experimental investigations into the training behavior of convolutional neural networks (CNNs), focusing on optimization strategies, activation functions, and weight initialization.

The goal is to connect the mathematical foundations of neural network training with empirical observations, examining how different design choices influence predictive performance, training stability, and computational efficiency.

Note: This repository is a clone of a similar private repo for a machine learning class (MATH161A: Mathematical Foundations of Machine Learning).

## Experiments

### 1. Activation Functions and Weight Initialization

**Notebook:** `prelu_he_initialization.ipynb`

This experiment investigates how activation functions and weight initialization methods affect the training behavior of a convolutional neural network on the CIFAR-10 dataset.

The investigation focuses on:

- Comparing ReLU, Leaky ReLU, and Parametric ReLU (PReLU).
- Examining He and Xavier initialization.
- Analyzing how initialization influences the variance of network activations.
- Comparing training performance across different configurations.

The experiment connects theoretical initialization principles with observed network behavior to explore how activation functions and initial weight distributions interact during training.

### 2. Large-Minibatch Stochastic Gradient Descent

**Notebook:** `large_minibatch_sgd.ipynb`

This experiment examines the effects of minibatch size on the training performance and computational efficiency of a convolutional neural network using the CIFAR-100 dataset.

The investigation focuses on:

- Comparing minibatch sizes of 32, 64, 128, 256, and 512.
- Evaluating fixed versus linearly scaled learning rates.
- Investigating gradual learning-rate warmup for larger minibatches.
- Measuring training throughput and validation accuracy.
- Connecting minibatch sampling and optimization behavior to their mathematical foundations.

The objective is to investigate whether learning-rate scaling and warmup can help compensate for the reduced number of parameter updates associated with larger minibatches.

## Methodology

Both investigations combine mathematical explanations with computational experiments implemented in Python and PyTorch.

The notebooks include experimental configurations, training and evaluation procedures, visualizations, and interpretations of the observed results.

The experiments are intended to investigate specific training behaviors under controlled settings rather than establish universally optimal neural network configurations.

## Reproducing the Experiments

The notebooks were developed for execution in Kaggle Notebooks with Python and PyTorch.

To reproduce an experiment:

1. Open the corresponding notebook in Kaggle or another compatible Jupyter environment.
2. Ensure that the required Python libraries and datasets are available.
3. Configure an appropriate execution device (CPU or GPU).
4. Execute the notebook cells in order.

Training times and measured throughput may vary depending on hardware, software versions, and runtime conditions.

## References

1. He, K., et al. (2015). *Delving Deep into Rectifiers: Surpassing Human-Level Performance on ImageNet Classification.* Proceedings of the IEEE International Conference on Computer Vision (ICCV), 1026–1034. https://arxiv.org/abs/1502.01852

2. Goyal, P., et al. (2017). *Accurate, Large Minibatch SGD: Training ImageNet in 1 Hour.* https://arxiv.org/abs/1706.02677
