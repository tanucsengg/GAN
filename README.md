## 1. GAN Implementation on MNSIT dataset
New framework for estimating generative models via an adversarial process, in which we simultaneously train two models: a generative model G that captures the data distribution, and a discriminative model D that estimates the probability that a sample came from the training data rather than G. The training procedure for G is to maximize the probability of D making a mistake. This framework corresponds to a minimax two-player game. In the space of arbitrary functions G and D, a unique solution exists, with G recovering the training data distribution and D equal to 1/2 everywhere. In the case where G and D are defined by multilayer perceptrons, the entire system can be trained with backpropagation.
Dataset: MINIST 
Number of Images:60,000
Optimiser: SGD
GAN: DCGAN
DCGAN is one of the popular and successful network designs for GAN. It mainly composes of convolution layers without max pooling or fully connected layers. It uses convolutional stride and transposed convolution for the down sampling and the up sampling. The figure below is the network design for the generator.

