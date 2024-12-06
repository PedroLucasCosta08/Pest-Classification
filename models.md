## Models
---

### torchvision

* AlexNet_Weights.IMAGENET1K_V1     56.522      61.1M

#### ResNet

| Model                             | Acc.    |   Params  |
|:----------------------------------|:--------|:----------|
| ResNet101_Weights.IMAGENET1K_V1   |  77.374 |     44.5M |
| ResNet101_Weights.IMAGENET1K_V2   |  81.886 |     44.5M |
| ResNet152_Weights.IMAGENET1K_V1   |  78.312 |     60.2M |
| ResNet152_Weights.IMAGENET1K_V2   |  82.284 |     60.2M |
| ResNet18_Weights.IMAGENET1K_V1    |  69.758 |     11.7M |
| ResNet34_Weights.IMAGENET1K_V1    |  73.314 |     21.8M |
| ResNet50_Weights.IMAGENET1K_V1    |  76.13  |     25.6M |
| ResNet50_Weights.IMAGENET1K_V2    |  80.858 |     25.6M |

#### VGG

| Model                             | Acc.    |   Params  |
|:----------------------------------|:--------|:----------|
| VGG11_BN_Weights.IMAGENET1K_V1    |  70.37  |    132.9M |
| VGG11_Weights.IMAGENET1K_V1       |  69.02  |    132.9M |
| VGG13_BN_Weights.IMAGENET1K_V1    |  71.586 |    133.1M |
| VGG13_Weights.IMAGENET1K_V1       |  69.928 |    133.0M |
| VGG16_BN_Weights.IMAGENET1K_V1    |  73.36  |    138.4M |
| VGG16_Weights.IMAGENET1K_V1       |  71.592 |    138.4M |
| VGG19_BN_Weights.IMAGENET1K_V1    |  74.218 |    143.7M |
| VGG19_Weights.IMAGENET1K_V1       |  72.376 |    143.7M |

#### Densenet

| Model                             | Acc.   |  Params |
|:----------------------------------|:-------|:--------|
| DenseNet121_Weights.IMAGENET1K_V1 | 74.434 |   8.0M  |
| DenseNet161_Weights.IMAGENET1K_V1 | 77.138 |  28.7M  |
| DenseNet169_Weights.IMAGENET1K_V1 | 75.6   |  14.1M  |
| DenseNet201_Weights.IMAGENET1K_V1 | 76.896 |  20.0M  |

### Timm

#### EfficientNet

| Model                  | Acc.      |    Params | Size      |
|:-----------------------|:----------|:----------|:----------|
| efficientnet_b0        |   77.71%  |    5.29 M |  20.39 MB |
| efficientnet_b1        |   78.71%  |    7.79 M |  30.04 MB |
| efficientnet_b2        |   80.38%  |    9.11 M |  35.08 MB |
| efficientnet_b3        |   82.08%  |   12.23 M |  47.08 MB |
 
#### MobileNet V3

| Model                  | Acc.      |    Params | Size       |
|:-----------------------|:----------|:----------|:-----------|
| mobilenetv3_large_100  |  75.77%   |     4.58M |   21.05 MB |

#### Vision Transformer

| Model                  | Acc.      |    Params | Size       |
|:-----------------------|:----------|:----------|:-----------|
| vit_small_patch16_224  |  77.85%   |   48.75 M |  186.00 MB |
| vit_base_patch16_224   |  81.78%   |   86.54 M |  330.25 MB |
| vit_large_patch16_224  |  83.06%   |  304.33 M |    1.16 GB |


## Observatins:


* BN is batch normalization