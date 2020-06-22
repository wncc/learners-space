## Week 2

Welcome to Week 2! Having laid the foundations of Machine Learning, this week we start exploring algorithms and concepts of Machine Learning. We discuss about the fudamentals of Machine Learning - Linear Regression and Logisitic Regression. We also talk about the importance of Data Cleaning for a Machine Learning Model. There is a good resource link to get hands on experience in Exploratory Data Analysis. This week, we also come up with an advanced topic for the interested ones - Generalised Linear Models.

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

* This **[link](https://www.coursera.org/learn/machine-learning/lecture/Z9DKX/gradient-descent-for-multiple-variables)** here explains an optimisation technique for Machine learning models, (Linear Regression in our case), known as **Gradient Descent** to reach at the minima of the Cost Function so as to arrive at the optimum parameters/weights, i.e., find a value of *Θ* (the weight vector) such that the prediction of our model is the most accurate. And this is what we mean by **Model Training**, provide training data to the model, then the model is optimized according to the training data, and the predictions become more accurate. This process is repeated every time we provide new training data to the model.
