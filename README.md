# Image-classification-of-lung-diseases
The fact that computers can see is just not that amazing anymore. But, the techniques for teaching a computer to do this are now simpler and more refined than ever. This post shows you how easy it is to build an image classifier. All you need is some basic python skills and at least a few hundred images.

The approach here uses Keras, which is emerging as the best library for building neural networks. The code here also assumes you are using Tensorflow as the underlying library.
## Data Pre-processing
Use glob function for collecting all image directories and resize them to a common size using openCV as by default VGG16 takes the image input size as (224,224).
We can use data augmentation if we have less number of images by using Image data generator which apply zoom, shear, rotation, filters etc to image so that we can generalize our model and reduce overfitting.
Divide the data into 3 catergories (Train, Val, Test) consists of (70%,20%,10%) of the data respectively.
## Build the model
We can use any type of CNN architectures like VGG16, Resnet50 etc or we can even do experimentation by building our CNN architecture.
Use dropout or BatchNormalization to reduce overfitting if have a very deep neural network.
## Inference
We can use openCV,matplotlib libraries to visualize the images that are classified and check for evaluation metrics.
