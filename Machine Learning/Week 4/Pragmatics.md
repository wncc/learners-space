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

## Regularisation  (To be Added Soon)
