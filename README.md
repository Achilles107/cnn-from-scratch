# cnn-from-scratch
Implemented Convolutional Neural Network from scratch. Used the MNIST dataset for the implementation.

# MNIST Data:

![Sample Data](https://github.com/Achilles107/cnn-from-scratch/blob/master/samplData.png)

# Summary of the Leaner:

Sequential
======================================================================
Layer (type)         Output Shape         Param #    Trainable 
======================================================================
Conv2d               [8, 14, 14]          72         True      
______________________________________________________________________
ReLU                 [8, 14, 14]          0          False     
______________________________________________________________________
BatchNorm2d          [8, 14, 14]          16         True      
______________________________________________________________________
Conv2d               [8, 14, 14]          576        True      
______________________________________________________________________
ReLU                 [8, 14, 14]          0          False     
______________________________________________________________________
BatchNorm2d          [8, 14, 14]          16         True      
______________________________________________________________________
Conv2d               [8, 14, 14]          576        True      
______________________________________________________________________
ReLU                 [8, 14, 14]          0          False     
______________________________________________________________________
BatchNorm2d          [8, 14, 14]          16         True      
______________________________________________________________________
MergeLayer           [8, 14, 14]          0          False     
______________________________________________________________________
Conv2d               [16, 7, 7]           1,152      True      
______________________________________________________________________
ReLU                 [16, 7, 7]           0          False     
______________________________________________________________________
BatchNorm2d          [16, 7, 7]           32         True      
______________________________________________________________________
Conv2d               [16, 7, 7]           2,304      True      
______________________________________________________________________
ReLU                 [16, 7, 7]           0          False     
______________________________________________________________________
BatchNorm2d          [16, 7, 7]           32         True      
______________________________________________________________________
Conv2d               [16, 7, 7]           2,304      True      
______________________________________________________________________
ReLU                 [16, 7, 7]           0          False     
______________________________________________________________________
BatchNorm2d          [16, 7, 7]           32         True      
______________________________________________________________________
MergeLayer           [16, 7, 7]           0          False     
______________________________________________________________________
Conv2d               [32, 4, 4]           4,608      True      
______________________________________________________________________
ReLU                 [32, 4, 4]           0          False     
______________________________________________________________________
BatchNorm2d          [32, 4, 4]           64         True      
______________________________________________________________________
Conv2d               [32, 4, 4]           9,216      True      
______________________________________________________________________
ReLU                 [32, 4, 4]           0          False     
______________________________________________________________________
BatchNorm2d          [32, 4, 4]           64         True      
______________________________________________________________________
Conv2d               [32, 4, 4]           9,216      True      
______________________________________________________________________
ReLU                 [32, 4, 4]           0          False     
______________________________________________________________________
BatchNorm2d          [32, 4, 4]           64         True      
______________________________________________________________________
MergeLayer           [32, 4, 4]           0          False     
______________________________________________________________________
Conv2d               [16, 2, 2]           4,608      True      
______________________________________________________________________
ReLU                 [16, 2, 2]           0          False     
______________________________________________________________________
BatchNorm2d          [16, 2, 2]           32         True      
______________________________________________________________________
Conv2d               [16, 2, 2]           2,304      True      
______________________________________________________________________
ReLU                 [16, 2, 2]           0          False     
______________________________________________________________________
BatchNorm2d          [16, 2, 2]           32         True      
______________________________________________________________________
Conv2d               [16, 2, 2]           2,304      True      
______________________________________________________________________
ReLU                 [16, 2, 2]           0          False     
______________________________________________________________________
BatchNorm2d          [16, 2, 2]           32         True      
______________________________________________________________________
MergeLayer           [16, 2, 2]           0          False     
______________________________________________________________________
Conv2d               [10, 1, 1]           1,440      True      
______________________________________________________________________
ReLU                 [10, 1, 1]           0          False     
______________________________________________________________________
BatchNorm2d          [10, 1, 1]           20         True      
______________________________________________________________________
Flatten              [10]                 0          False     
______________________________________________________________________

Total params: 41,132 

Total trainable params: 41,132 

Total non-trainable params: 0 

Optimized with 'torch.optim.adam.Adam', betas=(0.9, 0.99)

Using true weight decay as discussed in https://www.fast.ai/2018/07/02/adam-weight-decay/ 

Loss function : CrossEntropyLoss
