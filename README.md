# ResNet_MiniProject

**ResNet in Tensorflow for CIFAR-10** 


---


The following formulation is based on He et al.'s [paper](https://arxiv.org/abs/1512.03385).

General design decisions:

*   Full pre-activation residual block (see: [residual block variants](https://miro.medium.com/max/1400/1*M5NIelQC33eN6KjwZRccoQ.png))

*   Perform 1x1 convolution instead of padding input (projection shortcut) for matching output size 

Formulation based on [paper](https://arxiv.org/abs/1512.03385): 
*   1st layer is 3x3 convolutions 
*   Stack of 6n layers with 3x3 convolutions on feature maps of size {32,16,8} respectively (n = number of residual blocks) 
*   Ends with global average pooling, a FC layer, and softmax

About [CIFAR-10](http://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz):

*   Image size = 32x32
*   Label Dimension = 10 (classes)
*   60000 images total - 50000 training, 10000 testing 
*   5 training batches, 1 test batch

Google drive links to logs files:
*   [test_2_steps=10000](https://drive.google.com/drive/folders/1mFRgQPsh8C44Z1YlMq2MkNMxaBxw9jwc?usp=sharing)
*   [test_3_steps=20000](https://drive.google.com/drive/folders/133I5Y6YUzWwuf1BsG81Myk_U4y-_Xjq1?usp=sharing)
