# Welcome to Week 5 of LS Machine Learning! 
This week we will be covering the following topics: 
* Tensorflow framework
* Introduction to Recurrent Neural Networks 
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




