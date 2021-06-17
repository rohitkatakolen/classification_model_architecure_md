# VggNet model description

The VggNet architecture is the 1st runner up of ILSVR2014 in the classification task while the winner is GoogLeNet. Many modern image classification models are built on top of this architecture. 

# VggNet features

This network is characterized by its simplicity, using only 3×3 convolutional layers stacked on top of each other in increasing depth. Reducing volume size is handled by max pooling. 
To reduce the number of parameters, authors propose to use a small respective field to replace large one. Authors conclude:
    a. Incorporate multiple non-linear rectification layers instead of a single rectification layer are more discriminative.
    b. It helps to decrease the number of parameters while keeping performance. 

# VggNet model architecture

![](https://github.com/rohitkatakolen/classification_model_architecure_md/blob/main/img/vgg_models_architecture.png)



# Differnt models in VggNet
![](https://github.com/rohitkatakolen/classification_model_architecure_md/blob/main/img/densenet_models_architecture_2.png)

Each architecture consists of four DenseBlocks with varying number of layers. For example, the DenseNet-121 has [6,12,24,16] layers in the four dense blocks whereas DenseNet-169 has [6, 12, 32, 32] layers.


## VggNet Image Classification
| Model    | Nano (optimized) | TX2 (optimized)    | RTX (optimized)    |GTX-1650 (optimized)    |
|----------|:--------------:|:---------------:|:----------------:|:-----------------:|
| DenseNet |  |  |  |  |

