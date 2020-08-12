# Practical Aspects of Machine Learning Models - 1

So far, we have discussed about a multitude of models starting with Linear Regression model, Logisitic Regression, Decision trees to Neural Nets this week. As you 
might have seen so far, when we say 'fit the data', we mean some sort of a generalised fit. It is not desirable to fit the data perfectly. A model that accommodates 
each point of the curve may not be the optimal model for the data. There are several aspects of model fitting and there are factors that in some sense govern the 
desired accuracy of our model on the training data. Let us first get familiar with some concepts which we also explore in a greater depth in the coming weeks.  



## Generalization

Let us try to understand what we are actually trying to do with a Machine learning model. We train it on some data and want to use the same weights/parameters on 
some other data points to predict the target variable as accurately as possible. So when we say 'fit the data' perfectly, we don't actually mean to accommodate all 
the data points of our training data as perfectly as possible, what we actually mean is to figure out the underlying variations and try to generalise the data and 
accommodate the generalisation in our model so that accurate predictions can be made on unseen data.   

This leads us to kind of end results that are not desirable after training on the data - 

### Underfitting

It is a situation when the model doesn't fit the data properly. The values of the parameters in the parameters' space are far from global optima. It either means 
that the training of the model wasn't good or that the model is itself incapable of fitting the data points accurately. Predicting the line ( y = 2*x ) for the points 
lying roughly on ( y = x ) is an example for the former case wherein the slope can be optimised to fit the data accurately. Trying to fit a straight line on a data set 
that comes from some quadratic curve is an example for the second case. 

Such a result is obviously not desirable because it would lead to bad prediction results. 
Solution to this would be - 

* To figure out modifications in training
* Train for a longer duration to give more time to reach the global minima in the parameter space
* Change the model itself and find a suitable one to fit the data well

### Overfitting

It is a situation when the model fits the data points too accurately by keeping generalisation at the back seat. The model in the wake of reaching the global minima 
in the parameter space tries to accommodate the training data set points accurately and fails to predict the test data points accurately. Let us try to figure out 
why this can be the case. 

Let us say that we have data points coming from the distribution ( y = x**2 ), since the data cannot lie perfecty on the curve, there are some 
outliers to this generalisation. Now, since we defined our loss function to be mean squared error, so to minimise this, the model tries to accommodate this outlier 
on the curve too. So, maybe it tries to fit some higher degree complex polynomial on this data and it fails to identify the generalisation in the data that is a 
simple quadratic curve.  

At first such a result may appear good as the accuracy on the training set would be great but when tried on the test data is likely to give poor results.  

There are several solutions for this, many of which are model - specific

* Reduce the training time 
* Enrich the training set with a wide variety of examples
* Add Regularisation to the model

#### Useful Resources

* **[Underfitting and Overfitting Simplified](https://www.youtube.com/watch?v=BqzgUnrNhFM)**
* **[Underfitting vs Overfitting](https://www.analyticsvidhya.com/blog/2020/02/underfitting-overfitting-best-fitting-machine-learning/)**
* **[How to Deal with Underfitting and Overfitting](https://towardsdatascience.com/underfitting-and-overfitting-in-machine-learning-and-how-to-deal-with-it-6fe4a8a49dbf)**
* **[The Problem of Overfitting](https://www.youtube.com/watch?v=BqzgUnrNhFM)**

## Regularisation

Basically, this tends to reduce the magnitude of the weights/paramteres of the model in order to reduce the extent of overfitting and thus lead to better generalisations. This is called Regularisation. We look at a few techniques to regularise the network - 
* **Lasso Regression** - Also referred to as the **L1 regularisation**. This technique involves addition of magnitude of the weights to the loss function as a penalty so that they don't become large enough and overfit the data.  

* **Ridge Regression** - Also referred to as the **L2 regularisation**. Unlike the L1 method, this method adds the squared values of the weights to the loss function on a similar note.  

Let us try to understand what is it helpful in reducing overfitting. One of the popular ideas behind this is that adding that term leads to reduced magnitude of weights and that leads to lower value of activations. If you see the activation functions used, the graph is pretty much linear at values close to 0 and thus model becomes simpler and it is difficult for it to fit complicated functions and hence reduces overfitting.

#### Useful Resources

* **[Regularisation in Machine Learning](https://towardsdatascience.com/regularization-in-machine-learning-76441ddcf99a#:~:text=increasing%20model%20interpretability.-,Regularization,linear%20regression%20looks%20like%20this.)**

* Read the **[article](https://towardsdatascience.com/l1-and-l2-regularization-methods-ce25e7fc831c)** to get into the details of L1 and L2 regularisation techniques.  

#### Probabilistic Intrepretation of Regularisation (Optional)
There is a rigorous proof for Ridge Regression but that requires a bit of knowledge about statistics. Head **[here](https://www.quora.com/What-is-the-difference-between-Bayesian-and-frequentist-statisticians)** to get an overview of the statistics involved. Now, for those of you who read about Generalised Linear Models in Week 2 know the proof of how Linear Model Relations come up. There, we used the likelihood formula for the parameters but that was on the basis of Frequentistic Statistics, but if the same is done using the Bayesian Distribution, then in addition to the Standard Loss function, a **L2** loss shows up in the loss function. This can be in some sense related to **Maximum Likelihood Estimate** vs **Maximum A Posterior**  

#### Useful Resources 
* **[Probabilistic Interpretation of Regularisation](http://bjlkeng.github.io/posts/probabilistic-interpretation-of-regularization/)**

There are a lot more things in regularisation specific to neural nets. We will talk about them the next week after we have a clear understanding of neural networks.  
