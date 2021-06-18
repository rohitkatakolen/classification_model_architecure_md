# MobileNetV2 model description

MobileNetV2 from Google is particularly useful for mobile and embedded vision applications.

# MobileNetV2 features

MobileNet V2 is the successor of MobileNet V1 version
The architecute has following features:
    a. Smaller model size: Fewer number of parameters
    b. Smaller complexity: Fewer Multiplications and Additions (Multi-Adds)

MobileNetV2 has 3 types of convulution blocks - 

a. Depthwise separable convolutions layer - It does approximately the same thing as traditional convolution but is much faster.
b. Expansion layer - This converts a tensor with low number of dimensions to a tensor with higher number of dimensions.
c. Projection layer - It projects data with a high number of dimensions (channels) into a tensor with a much lower number of dimensions.

The expansion layer acts as an decompressor (like unzip) that first restores the data to its full form, then the depthwise layer performs whatever filtering is important at 
this stage of the network, and finally the projection layer compresses the data to make it small again.

![](https://github.com/rohitkatakolen/classification_model_architecure_md/blob/main/img/mobilenetv2_data_pass.png)

# MobileNetV2 model architecture

Basic block of MobileNetV2 - 
![](https://github.com/rohitkatakolen/classification_model_architecure_md/blob/main/img/mobilenetv2_architecure_block.png)


## MobileNetV2 Image Classification
| Model    | Nano (optimized) | TX2 (optimized)    | RTX (optimized)    |GTX-1650 (optimized)    |
|----------|:--------------:|:---------------:|:----------------:|:-----------------:|
| DenseNet |  |  |  |  |

