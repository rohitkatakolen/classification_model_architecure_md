# SqueezeNet model description

SqueezeNet: AlexNet-level accuracy with 50x fewer parameters

# SqueezeNet features

1. Replace 3×3 filters with 1×1 filters
2. Decrease the number of input channels to 3×3 filters
3. Downsample late in the network so that convolution layers have large activation maps

# SqueezeNet model architecture

Squeezenet fire module -  
![](https://github.com/rohitkatakolen/classification_model_architecure_md/blob/main/img/squeezenet_fire_module.png)

A Fire module is comprised of: a squeeze convolution layer (which has only 1×1 filters), feeding into an expand layer that has a mix of 1×1 and 3×3 convolution filters.

Squeezenet overall achitecture - 

![](https://github.com/rohitkatakolen/classification_model_architecure_md/blob/main/img/squeezenet_architecture.png)

## SqueezeNet Image Classification
| Model    | Nano (optimized) | TX2 (optimized)    | RTX (optimized)    |GTX-1650 (optimized)    |
|----------|:--------------:|:---------------:|:----------------:|:-----------------:|
| DenseNet |  |  |  |  |

