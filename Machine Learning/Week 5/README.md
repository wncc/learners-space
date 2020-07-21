# Welcome to Week 5 of LS Machine Learning! 
This week we will be covering the following topics: 
* Introduction to Tensorflow and Keras 
* Introduction to Convolutional Neural Networks
* Practice Assignment - Basic Image Classification in Tensorflow

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

Till now, you are familiar only with fully connected layers, where each input is mapped to every activation of the next hidden layer with a weight (parameter) associated with it. The total number of parameters between the input layer and the hidden layer thus become equal to the product of elements in both the layers. You are also aware the process of 'Back Propagation' deals with optimising the values of these parameters. Hence, larger the number of parameters of the model, longer the time it will take for training. 

Now let's say you were to do the same process described above, but with image pixel values as your input. Considering even a small image, of say **50x50** pixels, number of input variables will be equal to **2500**. And lets say you are mapping these input pixel values to a fully connected layer with **1000** elements. Obviously, you cannot directly map the input to a smaller feature space, since that will result in a lot of image features not getting learnt by your model, defeating the purpose of using a DNN. So, the number of parameters for this layer is equal to **2500 x 1000 = 2,500,000**. The number of parameters already cross a million and imagine what will happen with more layers. The total number of parameters to be trained will be huge! And remember, this is just for a **50x50** pixel input image. What if you were to use a **1024x1024** sized image? The training time for your model will be even larger this time and hence using fully connected layers is not an efficient approach to deal with image inputs. 
<br>This is where the concept of Convolutional Layers comes in, and a network comprised of convolutional layers (along with fully connected and other layers) is known as a **Convolutional Neural Network** (ConvNet). 

### Convolutional Layers 
Convolutional layers are specifically used in ConvNets when working with images. The use of a Convolutional layer instead of a fully connected layer results in significant decrease in the number of trainable parameters of the model without negligible loss in feature learning. The basic idea of a convolutional layer is to use a filter over the input image, where the filter is a 2D matrix custom designed to learn a particular feature (eg: a vertical edge). The output of the operation is another matrix but of reduced dimensions.
* Read about Convolutional layers from this detailed article - **[Convolutional Layer](https://cs231n.github.io/convolutional-networks/#conv)**
* You can also checkout this article for an alternate source - **[Convolution Reading](https://machinelearningmastery.com/convolutional-layers-for-deep-learning-neural-networks/)**
* Additionally, you can watch the following videos for a better understanding - **[Video #1](https://www.youtube.com/watch?v=XuD4C8vJzEQ&list=PLkDaE6sCZn6Gl29AoE31iwdVwSG-KnDzF&index=2), [Video #2](https://www.youtube.com/watch?v=am36dePheDc&list=PLkDaE6sCZn6Gl29AoE31iwdVwSG-KnDzF&index=3), [Video #3](https://www.youtube.com/watch?v=smHa2442Ah4&list=PLkDaE6sCZn6Gl29AoE31iwdVwSG-KnDzF&index=4), [Video #4](https://www.youtube.com/watch?v=tQYZaDn_kSg&list=PLkDaE6sCZn6Gl29AoE31iwdVwSG-KnDzF&index=5)**
* Checkout this video to get an idea of how to apply filter/kernels to multichannel RGB images - **[Convolution over volumes](https://www.youtube.com/watch?v=KTB_OFoAQcc&list=PLkDaE6sCZn6Gl29AoE31iwdVwSG-KnDzF&index=6)**

### Pooling Layers
Pooling layers are based on the same concept as convolutional layers, that is, even they perform a filtering operation on the input image matrix, but a pooling filter is not used to detect a particular feature. The aim of a pooling layer is to simply reduce the dimensions of the input matrix to reduce the number of trainable parameters and hence decrease the number of computations, without a huge loss in the features of the input image. Even though there is a trade off between the accuracy of the learned features and computation time, it is very common to make use of pooling layers since the latter is a bigger concern for deep learning models. Pooling layers can be of different types, such as, Max Pooling, Global Average pooling, etc.
* Read more about Pooling layers from this link - **[Pooling Layers](https://cs231n.github.io/convolutional-networks/#pool)**
* Watch the video for a better understanding - **[Pooling layers Video](https://www.youtube.com/watch?v=8oOgPUO-TBY&list=PLkDaE6sCZn6Gl29AoE31iwdVwSG-KnDzF&index=9)**

### ConvNets
Now that you are familiar with the different layers that any Convolutional Neural Network is comprised of, namely the Fully Connected Layer, Convolutional Layer and the Pooling Layer, let us look at some examples. 
* Go through this article which talks about ConvNet architectures in detail, along with the things you should keep in mind when desigining your own model architecture - **[ConvNet Architectures](https://cs231n.github.io/convolutional-networks/#architectures)**
* Additionally, go through these videos for a better grasp on ConvNets - **[Example ConvNet #1](https://www.youtube.com/watch?v=3PyJA9AfwSk&list=PLkDaE6sCZn6Gl29AoE31iwdVwSG-KnDzF&index=8), [Example ConvNet #1](https://www.youtube.com/watch?v=bXJx7y51cl0&list=PLkDaE6sCZn6Gl29AoE31iwdVwSG-KnDzF&index=10)** 

As you might have seen in the links, there are many pre-defined architectures which are widely used for many Deep Learning applications. Some of these are ResNet50, VGG16, Inception and many more. Try to find more information about these architectures and figure out the different layers that are being used in them. This will familiarise you with the ConvNet architectures used in common practice for different applications. 
<br> It is important to note here that these architectures are readily available as modules in the Keras' applications library, so you don't need to build these architectures from scratch! 

## Practice Assignment 
Finally, we will end this week's tutorial by performing an Image Classification task accomplished using Convolutional Neural Networks. Tensorflow officially provides many basic and advanced tutorials on different topics of Machine Learning. You can learn a lot about different Tensorflow and Keras functions just by following their notebooks step-by-step and referring to the official documentation wherever you get stuck. 

Head over to this link for a basic tutorial on Image Classification in Tensorflow using CNNs - **[Tensorflow Image Classification](https://www.tensorflow.org/tutorials/images/cnn)**

**Optionally**, you can also go through the tutorial below, which is also on Image classification, but adds more complexity to the task. It will help you visualize the concept of Overfitting on an actual dataset after you have trained the model and then elaborates on techniques to avoid it. But remember, this is an optional resource only meant for those who have completed and understood all the previous content before. - **[Image Classification Complex (Optional)](https://www.tensorflow.org/tutorials/images/classification#visualize_training_results)**


## Links to resources 
Many of the links provided above are from the [CNN Course on Coursera](https://www.coursera.org/programs/indian-institute-of-technology-bombay-gkhfq/browse?productId=kWGvJivBEeeW5RJUyz1uFA&productType=course&query=Convolutional+Neural+Networks&showMiniModal=true) (By Andrew Ng) and [Stanford's CS231n course](https://cs231n.github.io) on Convolutional Neural Networks. These courses are extremely detailed and act as a starting point for many ML enthusiasts. So it is recommended that you checkout the entire course if you want a deeper understanding of the underlying math of CNNs. 


We Hope that you enjoyed Week 5 of LS ML! 
<br>See you in Week 6! 




