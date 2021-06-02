# Resnet model family

ResNet, short for Residual Networks is a classic neural network used as a backbone for many computer vision tasks. This model was the winner of ImageNet challenge in 2015. The fundamental breakthrough with ResNet was it allowed us to train extremely deep neural networks with 150+layers successfully.

## Problem with deep neural networks

When we increase the number of layers significantly, there is a common problem in deep learning associated with that called Vanishing/Exploding gradient. This causes the gradient to become 0 or too large. Thus when we increases number of layers, the training and test error rate also increases.

## Intuition behind resnet blocks

<img src="img/residual_block.png">

ResNet blocks use a technique called skip connections . The skip connection skips training from a few layers and connects directly to the output.

The approach behind this type of network is that instead of layers learn the underlying mapping, we allow network fit the residual mapping. So, instead of say H(x), initial mapping, let the network fit, F(x) := H(x) – x which gives H(x) := F(x) + x.

The advantage of adding this type of skip connection is because if any layer hurt the performance of architecture then it will be skipped by regularization. So, this results in training very deep neural network without the problems caused by vanishing/exploding gradient.  The authors of the paper experimented on 100-1000 layers on CIFAR-10 dataset.

# ResNet model family

Image 2

Each ResNet block is either 2 layer deep (Used in small networks like ResNet 18, 34) or 3 layer deep( ResNet 50, 101, 152).

Image 3
