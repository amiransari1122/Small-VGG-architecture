# Small-VGG-architecture
A simple modified VGG convolution neural networks with smaller Conv layers to train faster for practice goals. Netwrok Smmary is given below. In this project Cifar10 dataset used to train VGG from TorchVision pytorch library.

----------------------------------------------------------------
        Layer (type)               Output Shape         Param #
================================================================
            Conv2d-1           [-1, 32, 32, 32]             896
              ReLU-2           [-1, 32, 32, 32]               0
       BatchNorm2d-3           [-1, 32, 32, 32]              64
            Conv2d-4           [-1, 32, 32, 32]           9,248
              ReLU-5           [-1, 32, 32, 32]               0
       BatchNorm2d-6           [-1, 32, 32, 32]              64
         MaxPool2d-7           [-1, 32, 16, 16]               0
            Conv2d-8           [-1, 64, 16, 16]          18,496
              ReLU-9           [-1, 64, 16, 16]               0
      BatchNorm2d-10           [-1, 64, 16, 16]             128
           Conv2d-11           [-1, 64, 16, 16]          36,928
             ReLU-12           [-1, 64, 16, 16]               0
      BatchNorm2d-13           [-1, 64, 16, 16]             128
        MaxPool2d-14             [-1, 64, 8, 8]               0
           Conv2d-15            [-1, 128, 8, 8]          73,856
             ReLU-16            [-1, 128, 8, 8]               0
      BatchNorm2d-17            [-1, 128, 8, 8]             256
           Conv2d-18            [-1, 128, 8, 8]         147,584
             ReLU-19            [-1, 128, 8, 8]               0
      BatchNorm2d-20            [-1, 128, 8, 8]             256
        MaxPool2d-21            [-1, 128, 4, 4]               0
           Linear-22                 [-1, 1024]       2,098,176
           Linear-23                   [-1, 10]          10,250
================================================================
Total params: 2,396,330
Trainable params: 2,396,330
Non-trainable params: 0
----------------------------------------------------------------
Input size (MB): 0.01
Forward/backward pass size (MB): 2.74
Params size (MB): 9.14
Estimated Total Size (MB): 11.90
----------------------------------------------------------------
