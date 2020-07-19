# Welcome to Week 5 of LS Machine Learning! 
This week we will be covering the following topics: 
* Tensorflow framework
* Introduction to Convolutional Neural Networks

## Tensorflow and Keras
Last week, you learned about Neural Networks, Backpropagation, Loss Function, Optimizers, Activation functions and how all of these are used together for training a Machine Learning model. But each and every function you defined was written from scratch in Python using classes. Tensorflow is an end-to-end open source tool developed by Google which contains pre-defined modules for all the different loss functions, optimisers, activation functions, layers, data pre-processing tools and much more which can speed up the process of performing machine learning by a huge amount.
<br>Even though all the modules and libraries can be accessed just using Tensorflow, you can also use the **Keras** API with the Tensorflow framework, which also contains pre-trained models like ResNet50, VGG16, etc. in addition to all the functions offered in Tensorflow. For this tutorial, we will be working with Tensorflow keras. 

To get started, first pip install tensorflow and keras and then simply import them in your code. 
~~~ 
pip install tensorflow
pip install keras
import tensorflow as tf
from tensorflow import keras
~~~
Note that you don't need to remember any of the syntax for importing different modules, just google whatever you need. The documentation provided by Tensorflow is already extremely detailed and easy to understand. 

## Convolutional Nerual Networks
### Introduction 
In the previous week, you studied about Neural Networks, specifically Feed Forward Neural Networks, in which you either have one or two hidden layers to map your input to the output. When several hidden layers are used in a Nerual Network, it is known as a **Deep Neural Network (DNN)** and this is where Deep Learning comes into the picture. A DNN is a basic unit of any Deep Learning architecture. 
<br> Till now, you are familiar only with fully connected layers, where each input is mapped to every activation of the next hidden layer with a weight (parameter) associated with it. The total number of parameters between the input layer and the hidden layer thus become equal to the product of elements in both the layers. You are also aware the process of 'Back Propagation' deals with optimising the values of these parameters. Hence, larger the number of parameters of the model, longer the time it will take for training. 
<br> Now let's say you were to do the same process described above, but with image pixel values as your input. Considering even a small image, of say **50x50** pixels, number of input variables will be equal to **2500**. And lets say you are mapping these input pixel values to a fully connected layer with **1000** elements. Obviously, you cannot directly map the input to a less number of elements, since that will result in a loss of minute features being learnt by your model, defeating the purpose of using a DNN. So, the number of parameters for this layer is equal to **2500 x 1000 = 2,500,000**. Now imagine using atleast 4 layers in your architecture. The total number of parameters to be trained will be huge! And remember, this is just for a **50x50** pixel input image. What if you were to use a **1024x1024** sized image? The training time for your model will be very large and hence this is not an efficient approach to deal with image inputs. 
This is where the concept of Convolutional Layers comes in, and a network comprised of convolutional layers (along with fully connected and other layers) is known as a **Convolutional Neural Network**. 
