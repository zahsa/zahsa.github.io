## VGG16
- ~138 milion parameters
- all conv layers are of size 3*3
- all max pool layers are of size 2*2, stride 2
- idea: all variables sized convolutional kernels used in AlexNet can be replicated by making use of multiple 3*3 kernels


## ResNet-18
- ~11 milion parameters
- attempts to find simpler mapping
- dealing with vanishing gradient problem when networks are deepers
- identity shortcut + projection shortcut
- filters of size 3*3
- residual block is repeated throughout the net

## Inception-v1 (GoogleNet)
- ~7 milion
- idea: larger kernels are preferred for more global features that are distributed over large area of image
- smaller kernels for detecting area-specific features
- For effective recogntion, we need kernels of different sizes
- inception instead of going deeper (in terms of number of layers) it goes wider.
- multiple kernels of different sizes are implemented within the same layer
- 1*1 conv blocks used for depth reduction
- 5*5 conv blocks captures global features
- 3*3 conv blocks captures distributed features
- max-pooling captures low-level features
- apply parallel filter operations on the input from previous layers
  
