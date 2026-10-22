# Biweekly Report 2

## Candido Seneriches IV

### prelu_he_initialization.ipynb
In this file, I integrated the activation functions ReLU, Leaky ReLU, and PReLU, as well as the weight initialization methods Xavier initialization and He initialization into a convolutional neural network in order to examine the effect if any of these features on the performance of said CNN.

### large_minibatch_sgd.ipynb
In this file, I investigated the effects of different minibatch sizes on the training performance and computational efficiency of a convolutional neural network using the CIFAR-100 dataset. I also experimented with linear learning-rate scaling and gradual learning-rate warmup to examine whether these techniques could improve the performance of larger minibatches when training with stochastic gradient descent (SGD).

### References
He, Kaiming, et al. “Delving Deep into Rectifiers: Surpassing Human-Level Performance on ImageNet Classification.” *Proceedings of the IEEE International Conference on Computer Vision (ICCV)*, 2015, pp. 1026–1034. https://arxiv.org/abs/1502.01852.

Goyal, Priya, et al. “Accurate, Large Minibatch SGD: Training ImageNet in 1 Hour.” *arXiv*, 2017, https://arxiv.org/abs/1706.02677.