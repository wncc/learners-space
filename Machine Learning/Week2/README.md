# Week 2

Welcome to Week 2! Having laid the foundations of Machine Learning, this week we start exploring algorithms and concepts of Machine Learning. We discuss about the fudamentals of Machine Learning - 

* Linear Regression
* Logisitic Regression
* Importance of Data Cleaning and Pre-Processing
* Exploratory Data Analysis 
* Generalised Linear Models (Advanced optional content)

## Linear Regression

Linear Regression is one of the most fundamental models in Machine Learning. It assumes a linear relationship between the input variables *(x)* and the single output variable *(y)*. Formally stating, *(y)* can be calculated from a linear combination of the input variables *(x)*. 

When we have a single variable *(x)* as the input, the model is called as **Simple Linear Regression** and when we have multiple input variables, the model is called **Multiple Linear Regression**.  
In Machine learning, the input variable *(x)* corresponds to the features of our dataset, for eg. when we are predicting housing prices from a dataset, the features of the dataset will be Area of the house, Locality, etc. and the output variable *(y)* in this case will be the housing price. The general representation of a Simple Linear Regression Model is -
                                                
                                                y = θ(0) + θ(1)*x

where *θ(0)* is known as the **bias term**, and *θ* in general is called as the **weight vector**. This **[link](https://www.coursera.org/learn/machine-learning/lecture/db3jS/model-representation)** here explains in detail how we arrived at such a representation of the model. For multiple linear regression, the equation changes as - 

                                                y = transpose(Θ)*(X) 

where *X* is a vector containing all the features and *Θ* is a vector containing all the corresponding weights i.e. the parameters of the linear model.  

We define a function called the **Cost Function** that accounts for the prediction errors of the model. We try to minimize the cost function so that we can obtain a model that fits the data as good as possible. To reach the optima of the cost function, we employ a method that is used in almost all of machine learning called **Gradient Descent**.

* This **[article's](http://www.stat.cmu.edu/~cshalizi/mreg/15/lectures/03/lecture-03.pdf)** sections 2 and 3 explain the concept of Linear Regression as a Statistical Model, where you can calculate certain statistical quantities to determine and improve the accuracy of your model. This is known as **Optimisation**.

* This **[link](https://www.coursera.org/learn/machine-learning/lecture/Z9DKX/gradient-descent-for-multiple-variables)** here explains an optimisation technique for Machine learning models, (Linear Regression in our case), known as **Gradient Descent** to reach at the minima of the **[Cost Function](https://www.coursera.org/lecture/machine-learning/cost-function-rkTp3)** so as to arrive at the optimum parameters/weights, i.e., find a value of *Θ* (the weight vector) such that the prediction of our model is the most accurate. And this is what we mean by **Model Training**, provide training data to the model, then the model is optimized according to the training data, and the predictions become more accurate. This process is repeated every time we provide new training data to the model.


### Segmented Regression

It is also referred to as **Piecewise Regression** or **Broken Stick Regression**. Unlike standard Linear Regression, we fit separate line segments to intervals of independent variables. This is usually more accurate than the conventional Linear Regression. Also, it becomes important to understand that despite its accuracy, its computational efficiency is lesser than the latter.  
The points where the data is split are called **Break Points**. 

* To get an overview of the concepts, go through **[this](https://storybydata.com/datacated-challenge/piecewise-linear-regression/)** article.
* To delve deeper into the mathematical aspects and get hands on experience, go through **[this](https://www.fs.fed.us/rm/pubs/rmrs_gtr189.pdf)**.

To a limited extent, this kind of regression is useful to fit data that is not linear in nature.

## Logistic Regression

Logistic regression is a classifier that uses regression to obtain the probability of the input data belonging to one of various classes. Unlike Linear Regression, where the target values are continuous real valued, the target variables here are drawn from a finite set of discrete values. Formulation of logistic regression can be made where the parameters are estimated using gradient descent.  

* This **[article](https://towardsdatascience.com/logistic-regression-detailed-overview-46c4da4303bc)** covers the major aspects of Logistic Regression and should give you a firm grasp on the mathematics behind this algorithm

### Multinomial Logistic Regression

Logistic regression can be binary or multinomial in nature. The **multinomial logistic regression** is also termed as **Softmax Regression**. Go through this **[article](https://stats.idre.ucla.edu/stata/dae/multinomiallogistic-regression/)** to go deeper into the concepts of Multinomial Logistic Regression. 
 
## Exploratory Data Analysis

Last week, we learned about Data Visualisation and Exploration. To get hands on experience on Data Analysis on Regression and Classification, refer to the links below - 
* **[Regression](https://github.com/MicrosoftLearning/Principles-of-Machine-Learning-Python/blob/master/Module2/VisualizingDataForRegression.ipynb)**
* **[Classification](https://github.com/MicrosoftLearning/Principles-of-Machine-Learning-Python/blob/master/Module2/VisualizingDataForClassification.ipynb)**

## Generalised Linear Models (Optional)

On a very high level, Generalised Linear Models (GLM) are a superclass of all linear models including Linear and Logistic Regression that we talked about earlier. 

* Linear Regression is based on the assumption that the data assumes **Gaussian/Normal Distribution**.
* Binary Logistic Regression is based on the assumption that data assumes **Bernoulli Distribution**.

GLM's are based on Exponential Family Functions. **[Exponential Family](https://en.wikipedia.org/wiki/Exponential_family)** includes these two and a lot of other distributions of data that we talked about in week 1. So therefore GLM's serve as a generalisation of all linear models. To get a firm hold on generalised linear models, head **[here](https://towardsdatascience.com/generalized-linear-models-9cbf848bb8ab)**.
