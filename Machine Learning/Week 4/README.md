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

## FeedForward Neural Networks
The feedforward neural network was the first and simplest type of artificial neural network devised. In this network, the information moves in only one direction, forward, from the input nodes, through the hidden nodes (if any) and to the output nodes. There are no cycles or loops in the network. If we include loops, then it becomes **Recurrent Neural Network** which we'll learn in the upcoming week.

### **Forward Propagation**: <br/>
To put it simply, the process that runs inside a neuron for forward propagation is, the neuron takes n input data (training examples) x1, x2,..., xn and first assigns random weights and biases to all the input variables and calculate their weighted sum Z, and further pass it inside an activation function, g(x) such as a sigmoid (later we'll also talk about other alternatives for it),giving g(Z) = A. 
<br/>
Similarly, we calculate this activation, A for all the neurons in all the layers. The activations of the previous layer act as input data for the next layer and the activation of the last layer gives the output, y^(y-hat)
* Refer to this [3blue1brown video](https://www.youtube.com/watch?v=aircAruvnKk) to have a good visualisation
* Refer to this [article](https://towardsdatascience.com/forward-propagation-in-neural-networks-simplified-math-and-code-version-bbcfef6f9250) to understand more and implement code as well.
<br/><br/>
**Activation Functions** <br/>
We can use different types of activation functions such as sigmoid, tanh, Relu (rectified linear unit), leaky relu.
Refer to [this](https://www.analyticsvidhya.com/blog/2020/01/fundamentals-deep-learning-activation-functions-when-to-use-them/) to know about all of them.
Though, we generally prefer tanh over sigmoid since, both have similar properties, but tanh gives output whose mean can be centralised to 0 and has some other benefits which can be seen in [this](https://www.youtube.com/watch?v=nD5ag-Q1sms&t=405s) video.
Both of these activation functions, share one disadvantage that the slope tends to 0 when the numbers are very large or very small, thus the process of making improvememts slows down here, the leaky Relu function serves as a benefit in this case as it's slope never collapses. However, for practical purposes even relu function works well. 
<br/> While using for classification, we prefer the output of the last layer to be between 0 and 1, thus we use L-1 layers with relu activation and the last year with sigmoid activation for good results in a L layer NN.
Refer to [this](https://www.youtube.com/watch?v=G6djH3I0rG0&list=PLreVlKwe2Z0TTN9vNEsMhA2JVswctec2g) playlist to have a good idea about this.

<br/><br/>
By now, our model has made it's first prediction, but this was with random weights and biases, hence the results were very random, we need to train our model. Now, to begin it's training the model must know where it went wrong. thus it needs a function to compute loss.

**Optimization Problem**<br/>
Typically, a neural network model is trained using the gradient descent optimization algorithm and weights are updated using the backpropagation of error algorithm.The gradient descent algorithm seeks to change the weights so that the next evaluation reduces the error, meaning the optimization algorithm is navigating down the gradient (or slope) of error.Now that we know that training neural nets solves an optimization problem, we can look at how the error of a given set of weights is calculated.<br/>

### **Loss Function**<br/>
With neural networks, we seek to minimize the error. As such, the objective function is often referred to as a cost function or a loss function and the value calculated by the loss function is referred to as simply “loss.”

**Maximum Likelihood And Cross Entropy** <br/>
Maximum likelihood seeks to find the optimum values for the parameters by maximizing a likelihood function derived from the training data.<br/>
When modeling a classification problem where we are interested in mapping input variables to a class label, we can model the problem as predicting the probability of an example belonging to each class. In a binary classification problem, there would be two classes, so we may predict the probability of the example belonging to the first class.<br/>
Therefore, under maximum likelihood estimation, we would seek a set of model weights that minimize the difference between the model’s predicted probability distribution given the dataset and the distribution of probabilities in the training dataset. This is called the cross-entropy. <br/> <br/>

**Cross Entropy Loss and Mean Squared Loss(MSE)** are the losses we use of classification and regression problems respectively. To know the reasons behind chck this [video](https://www.youtube.com/watch?v=2ca_K2rgNVA). PS: since, this is a nptel video i would suggest watching on 1.5x speed or higher xD

### **Back


