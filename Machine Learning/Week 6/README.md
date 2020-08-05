# Week 6

This week we talk a lot about the pragmatics of Machine Learning/Deep Learning and explore the various techniques that enhance performance of our models greatly. 

## Intialisation

Correct initialisation of weights in a neural net is extremely important for an efficient training of a neural net. There are several ways to initialise the weights which we discuss below - 

### Zero Initialisation

We can initialise all the weights and baises of a network to be 0. Though this might seem okay at the first sight but this poses a big hindernace to the learning of a neural net. If two weights associated with a neuron are same then they continue to have the same value throughout as the derivative will be the same during entire training. This limits the learning of a neural net as the neurons don't learn different aspects of the data. So initialising two weights with the same value is not at all desirable and initialising all weights to 0 makes your neural net worthless. Although it is okay to initialise biases to the same value (including 0).

### Random Initialisation

As we have seen earlier, assigning same values to weights can hamper performance, so a solution to fix this can be to initialise weights randomly (say with a given mean and variance). Now, this random initialisation when done with different values of variance and mean 0 can lead to different kinds of initialisation techniques as described below - 

#### He Initialisation

This initialisation technique multiplies a dynamic number for each layer of the neural net, in particular it is proportional to the inverse square root of the number of incoming neurons. Read **[this](https://medium.com/@prateekvishnu/xavier-and-he-normal-he-et-al-initialization-8e3d7a087528)** for more info.

#### Xavier Initialisation

This is specifically for the tanh activation function, similar to the He Initialisation, the technqiue involves multiplication with a number proportional to the inverse square root of the number incoming neurons. Though the constants differ by the a factor of square root of 2. Read **[this](https://medium.com/@prateekvishnu/xavier-and-he-normal-he-et-al-initialization-8e3d7a087528)** for more info.

There are some techniques that involve multiplcation with a constant inversely proportional to the square root of sum of the number incoming and outgoing neurons. This proves to be a better initialisation stratergy for neural nets. 

### Uniform Initialisation

Similar to the logic behind random initialisation, one can also think about initialising weights drawn from a uniform distribution with a specific mean and variance. 

#### Glorot Uniform Intialisation

The weights are drawn from a uniform distribution with a specific variance. The details of which can be read in the resources provided below. 

### Why so Many Intialisation Techniques

Let us try to understand why are there so many intialisation techniques and how to think of them as special cases of a standard thing.

The baisc funda is that normalised inputs with mean 0 is always desirable for a neural net to be trained efficiently as it makes the optimization terrain more symmetrical with respect to the input features. On a similar note, it is desirable to make the derivatives normalised with mean 0 because that helps in faster training. So, the intialisation stratergy is to try to maintain that thing by assinging good intial values to the weights. So, there are two things to this - 

* Incoming neurons are related to normalised derivatives
* Outgoing neurons are related to the normalised activation values (inputs)

So, now, the various initialisation stratergies are associated with this fact that some of them use only the first condition, some of them the second one and some of them combine the two conditions. Also, depending upon the fact whether the technique draws values from a uniform or random distribution, one can derive these variance values. So in effect, at the heart of all initialisation techniques lies the two fundae mentioned above.

### Useful Resources

There are several articles one can read to get a grip on this technique. Also, links to two research papers have also been added for the interested people.

* **[Weight Initialisation Techniques](https://towardsdatascience.com/weight-initialization-techniques-in-neural-networks-26c649eb3b78)**
* **[Journey of Initialisation in Neural Nets](https://towardsdatascience.com/weight-initialization-in-neural-networks-a-journey-from-the-basics-to-kaiming-954fb9b47c79)**
* **[Research Paper on Glorot Initialisation](http://proceedings.mlr.press/v9/glorot10a/glorot10a.pdf)**
* **[Xavier and He Initialisation](https://medium.com/@prateekvishnu/xavier-and-he-normal-he-et-al-initialization-8e3d7a087528)**
* **[Mathematical Aspects of Initialisation](https://mmuratarat.github.io/2019-02-25/xavier-glorot-he-weight-init)**
* **[Research Paper on Exploring Initialisation Stratergies on Several Activation Functions](https://arxiv.org/pdf/1704.08863.pdf)**

## Dropouts

We studied earlier how Neural Nets and any machine learning model in general is prone to overfitting. Dropouts are an ingenius way to prevent this in the case of neural nets. Basically, some of the neurons are turned off in some sense at every forward pass during training. What is done is that the activation of some of the neurons of the network are set to 0 for one forward pass. This disallows any neuron to specialise in some aspect of the data that in turn reduces overfitting by allowing several neurons in the layer to learn things. Hence the learning gets distributed which leads to better generalisations. 

Basically, to implement this, a probabiity value is fixed and it is with this probability for every neuron that it is turned on or off.  

This technique has become really popular recently and the good thing is that the frameworks like Tensorflow already have Dropouts implemented that reduces the burden of implementing this.  

To read more about Dropouts, go through the following links - 

* **[Dropouts](https://medium.com/@amarbudhiraja/https-medium-com-amarbudhiraja-learning-less-to-learn-better-dropout-in-deep-machine-learning-74334da4bfc5)**
* **[Math Behind Dropouts](https://towardsdatascience.com/simplified-math-behind-dropout-in-deep-learning-6d50f3f47275)** (Advanced Content)
