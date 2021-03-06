# 其他模型

## 概述
正在持续更新中......

DarkNet53在预测时，图像的crop_size设置为256，resize_short_size设置为256；其余模型在预测时，图像的crop_size设置为224，resize_short_size设置为256。


## 精度、FLOPS和参数量

| Models                    | Top1   | Top5   | Reference<br>top1 | Reference<br>top5 | FLOPS<br>(G) | Parameters<br>(M) |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| AlexNet                   | 0.567  | 0.792  | 0.5720            |                   | 1.370        | 61.090            |
| SqueezeNet1_0             | 0.596  | 0.817  | 0.575             |                   | 1.550        | 1.240             |
| SqueezeNet1_1             | 0.601  | 0.819  |                   |                   | 0.690        | 1.230             |
| VGG11                     | 0.693  | 0.891  |                   |                   | 15.090       | 132.850           |
| VGG13                     | 0.700  | 0.894  |                   |                   | 22.480       | 133.030           |
| VGG16                     | 0.720  | 0.907  | 0.715             | 0.901             | 30.810       | 138.340           |
| VGG19                     | 0.726  | 0.909  |                   |                   | 39.130       | 143.650           |
| DarkNet53                 | 0.780  | 0.941  | 0.772             | 0.938             | 18.580       | 41.600            |
| ResNet50_ACNet            | 0.767  | 0.932  |                   |                   | 10.730       | 33.110            |
| ResNet50_ACNet<br>_deploy | 0.767  | 0.932  |                   |                   | 8.190        | 25.550            |


## FP16预测速度

| Models                    | batch_size=1<br>(ms) | batch_size=4<br>(ms) | batch_size=8<br>(ms) | batch_size=32<br>(ms) |
|:--:|:--:|:--:|:--:|:--:|
| AlexNet                   | 0.684                | 0.740                | 0.810                | 1.481                 |
| SqueezeNet1_0             | 0.545                | 0.841                | 1.146                | 3.501                 |
| SqueezeNet1_1             | 0.473                | 0.575                | 0.805                | 1.862                 |
| VGG11                     | 1.096                | 1.655                | 2.396                | 6.728                 |
| VGG13                     | 1.216                | 2.059                | 3.056                | 9.468                 |
| VGG16                     | 1.518                | 2.594                | 4.019                | 12.145                |
| VGG19                     | 1.817                | 3.124                | 4.886                | 14.958                |
| DarkNet53                 | 2.150                | 2.627                | 3.422                | 10.092                |                     |
| ResNet50_ACNet<br>_deploy | 2.748                | 3.178                | 3.823                | 8.369                 |


## FP32预测速度

| Models                    | batch_size=1<br>(ms) | batch_size=4<br>(ms) | batch_size=8<br>(ms) | batch_size=32<br>(ms) |
|:--:|:--:|:--:|:--:|:--:|
| AlexNet                   | 0.682                | 0.875                | 1.196                | 3.196                 |
| SqueezeNet1_0             | 0.530                | 1.072                | 1.652                | 5.338                 |
| SqueezeNet1_1             | 0.439                | 0.787                | 1.164                | 2.973                 |
| VGG11                     | 1.575                | 3.638                | 6.427                | 23.227                |
| VGG13                     | 1.859                | 4.832                | 8.832                | 32.946                |
| VGG16                     | 2.316                | 6.420                | 11.936               | 44.719                |
| VGG19                     | 2.775                | 8.013                | 14.925               | 57.272                |
| DarkNet53                 | 2.648                | 5.727                | 9.616                | 33.664                |                     |
| ResNet50_ACNet<br>_deploy | 4.544                | 6.873                | 9.627                | 28.283                |
