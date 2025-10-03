# TSAI-Assignment-4
#### Objective
Achieve 95% test accuracy in the first epoch with fewer than 25000 parameters

#### Model Architecture
----------------------------------------------------------------
        Layer (type)               Output Shape         Param #
================================================================

            Conv2d-1           [-1, 16, 26, 26]             160
              ReLU-2           [-1, 16, 26, 26]               0
            Conv2d-3           [-1, 32, 24, 24]           4,640
              ReLU-4           [-1, 32, 24, 24]               0
         MaxPool2d-5           [-1, 32, 12, 12]               0
            Conv2d-6           [-1, 32, 12, 12]           1,056
              ReLU-7           [-1, 32, 12, 12]               0
            Conv2d-8           [-1, 16, 10, 10]           4,624
              ReLU-9           [-1, 16, 10, 10]               0
           Conv2d-10              [-1, 1, 8, 8]             145
             ReLU-11              [-1, 1, 8, 8]               0
           Linear-12                   [-1, 10]             650
================================================================
Total params: 11,275
Trainable params: 11,275
Non-trainable params: 0
Train set accuracy: 84.08%
Test set accuracy: 95.75%

#### Training Logs
EPOCH: 0
Loss=0.14004863798618317 Batch_id=937 Accuracy=84.08: 100%|█| 938/938 [00:38<00:

Test set: Average loss: 0.1380, Accuracy: 9575/10000 (95.75%)

#### Training Details
Optimizer: SGD with learning rate 0.02 and momentum 0.9
Batch Size: 128 (if CUDA available) or 64
Epochs: 1