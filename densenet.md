# DenseNet model family

The DenseNet architecture is all about modifying this standard CNN architecture. In a DenseNet architecture, each layer is connected to every other layer, hence the name Densely Connected Convolutional Network.  

# DenseNet features

In DenseNet models, for each layer, the feature maps of all the preceding layers are used as inputs, and its own feature maps are used as input for each subsequent layers. This is done to enable maximum information flow between the layers of the network. To preserve the feed-forward nature, each layer obtains inputs from all the previous layers and passes on its own feature maps to all the layers which will come after it. Unlike Resnets it does not combine features through summation but combines the features by concatenating them. 

# DenseNet model architecture

![](https://github.com/rohitkatakolen/classification_model_architecure_md/blob/main/img/densenet_architecture.png)

Each architecture consists of four DenseBlocks with varying number of layers. For example, the DenseNet-121 has [6,12,24,16] layers in the four dense blocks whereas DenseNet-169 has [6, 12, 32, 32] layers.




## DenseNet Image Classification
| Model    | Nano (optimized) | TX2 (optimized)    | RTX (optimized)    |GTX-1650 (optimized)    |
|----------|:--------------:|:---------------:|:----------------:|:-----------------:|
| DenseNet |  |  |  |  |

