# Week 4

Welcome to Week 4! This week you are going to develop your understanding about neural networks and deep learning. 

Last week you studied about various machine learning algorithms.It’s a pertinent question. There is no shortage of machine learning algorithms so why should we gravitate towards deep learning algorithms? What do neural networks offer that traditional machine learning algorithms don’t?
### Why are neural nets preferred over traditional machine learning algorithms ?
Well, here are two key reasons why researchers and experts tend to prefer Deep Learning over Machine Learning:
* **Decision Boundary:** In the case of classification problems, the algorithm learns the function that separates 2 classes, this is known as a Decision boundary.This [video](https://www.coursera.org/lecture/machine-learning/decision-boundary-WuL1H) beautifully explains about decision boundaries and some good examples.<br/> ***Every Machine Learning algorithm is not capable of learning all the functions. This limits the problems these algorithms can solve that involve a complex relationship whereas Neural Nets can compute any function.*** <br/> OPTIONAL: If you wish to see the proof behind the same, refer to this [link](http://neuralnetworksanddeeplearning.com/chap4.html) for intuitive proof.

* **Feature Engineering:** Feature engineering is a key step in the model building process. It is a two-step process:
   * Feature extraction: In feature extraction, we extract all the required features for our problem statement
   * Feature selection: In feature selection, we select the important features that improve the performance of our machine learning or deep learning model.<br />
Consider an image classification problem. Extracting features manually from an image needs strong knowledge of the subject as well as the domain. It is an extremely time-consuming process. Thanks to Deep Learning, we can automate the process of Feature Engineering! All you need to do is just enter raw data, and the neural nets will classify it into features with appropiate weights on it's own.
<br/>
This week, we'll study about feedforward neural networks <br/>

### FeedForward Neural Networks
The feedforward neural network was the first and simplest type of artificial neural network devised. In this network, the information moves in only one direction, forward, from the input nodes, through the hidden nodes (if any) and to the output nodes. There are no cycles or loops in the network. If we include loops, then it becomes **Recurrent Neural Network** which we'll learn in the upcoming week.

**Forward Propagation**: <br/>
To put it simply, the process that runs inside a neuron for forward propagation is, the neuron takes n input data (training examples) x1, x2,..., xn and first assigns random weights to all the input variables and calculate their weighted sum Z, and further pass it inside an activation function, g(x) such as a sigmoid (later we'll also talk about other alternatives for it),giving g(Z) = A. 
<br/>
Similarly, we calculate this activation, A for all the neurons in all the layers. The activations of the previous layer act as input data for the next layer and the activation of the last layer gives the output.
* Refer to this [3blue1brown video](https://www.youtube.com/watch?v=aircAruvnKk) to have a good visualisation


