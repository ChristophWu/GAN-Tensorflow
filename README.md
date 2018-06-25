# GAN-Tensorflow

## Introduction
In this exercise, I will implement a Deep Convolutional Generative Network (DCGAN) to synthesis images by using the same 
animation face dataset.

## Structure
<img src="https://github.com/ChristophWu/GAN-Tensorflow/blob/master/material/structure.png" width="600"/>

## Objective function
<img src="https://github.com/ChristophWu/GAN-Tensorflow/blob/master/material/objective.png" width="500"/>

## Implementation
- utils.py is used to merge pictures into one picture
- dataset.py is used to cut the dataset into minibatches
- open terminal and python dagan.py to implement

## Results
- learning curve
<img src="https://github.com/ChristophWu/GAN-Tensorflow/blob/master/material/learning_curve.png" width="500"/>

- some examples of detected and undetected images
<img src="https://github.com/ChristophWu/GAN-Tensorflow/blob/master/material/DCGAN_generation_animation.gif" width="500"/>

## Tips
- Training procedure of GANs is unstable, when visualizing the loss curve you can do moving average every N steps 
(smooth the curve) to observe the trend easily.
- Optimizer such as Adam or RMSProp is recommended. SGD may take more iterations to converge.
- Set diﬀerent learning rates for G and D. Usually, learning rate of D could be smaller than G.
- Suggest training the model for about 100 to 150 epochs.
-  Batch normalization is useful for training neural network.

