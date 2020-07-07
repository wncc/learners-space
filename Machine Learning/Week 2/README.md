# Week 2

Welcome to Week 2! Having laid the foundations of Machine Learning, this week we start exploring algorithms and concepts of Machine Learning. We discuss about the fudamentals of Machine Learning - 

* **[Linear Regression](#linear-regression)**
* **[Segmented Regression](#segmented-regression)**
* **[Locally Weighted Regression](#locally-weighted-regression)**
* **[Logistic Regression](#logistic-regression)**
* **[Naive Bayes Classifier](#naive-bayes-classifier)**
* **[Exploratory Data Analysis](#exploratory-data-analysis)**
* **[Data Pre-Processing](#data-pre-processing)**
* **[Generalised Linear Models](#generalised-linear-models)** (Advanced optional content)

First we shall go into Machine Learning models for estimation of values. This is termed as regression. A good example would be using regression to obtain the least square fit line equation which we all have used in PH117 to obtain a good estimate of a linear model of the data points given. There are other models as well however linear regression is the simplest.  

## Linear Regression

Linear Regression is one of the most fundamental models in Machine Learning. It assumes a linear relationship between target variable *(y)* and predictors (input variables) *(x)*. Formally stating, *(y)* can be estimated assuming a linear combination of the input variables *(x)*. 

When we have a single predictor as the input, the model is called as **Simple Linear Regression** and when we have multiple predictors, the model is called **Multiple Linear Regression**.  
The input variable *(x)* is a vector of the features of our dataset, for eg. when we are predicting housing prices from a dataset, the features of the dataset will be Area of the house, Locality, etc. and the output variable *(y)* in this case will be the housing price. The general representation of a Simple Linear Regression Model is -
                                                
                                                y = θ(0) + θ(1)*x

where *θ(0)* is known as the **bias term**, and *θ* in general is called as the **weight vector**, there are the parameters of the linear regression model. This **[video](https://www.coursera.org/learn/machine-learning/lecture/db3jS/model-representation)** gives a detailed explanation of how we arrived at this representation. For multiple linear regression, the equation modifies to - 

                                                y = transpose(Θ)*(X) 

where *X* is a vector containing all the features and *Θ* is a vector containing all the corresponding weights (bias and weights both) i.e. the parameters of the linear model. Also note that *X* here has an additonal feature - the constant term 1 which accounts for the intercept of the linear fit.

We define a function called the **Cost Function** that accounts for the prediction errors of the model. We try to minimize the cost function so that we can obtain a model that fits the data as good as possible. To reach the optima of the cost function, we employ a method that is used in almost all of machine learning called **Gradient Descent**.  

---

#### Note

The relationship established between the target and the predictors is a statistical relation and not determinsitic. A deterministic relation is possible only when the data is actually prefectly linear.

---

#### Useful Resources

* **[Overview of Gradient Descent](https://medium.com/@saishruthi.tn/math-behind-gradient-descent-4d66eb96d68d)**

* This **[video](https://www.coursera.org/learn/machine-learning/lecture/Z9DKX/gradient-descent-for-multiple-variables)** here explains an optimisation technique for Machine learning models, (Linear Regression in our case), known as **Gradient Descent** to reach at the minima of the **[Cost Function](https://www.coursera.org/lecture/machine-learning/cost-function-rkTp3)** so as to arrive at the optimum parameters/weights, i.e., find a value of *Θ* (the weight vector) such that the prediction of our model is the most accurate. And this is what we mean by **Model Training**, provide training data to the model, then the model is optimized according to the training data, and the predictions become more accurate. This process is repeated every time we provide new training data to the model.  
 
* (Optional) This **[article's](http://www.stat.cmu.edu/~cshalizi/mreg/15/lectures/03/lecture-03.pdf)** sections 2 and 3 explain the concept of Linear Regression as a Statistical Model, where you can calculate certain statistical quantities to determine and improve the accuracy of your model. This is known as **Optimisation**.


## Segmented Regression

It is also referred to as **Piecewise Regression** or **Broken Stick Regression**. Unlike standard Linear Regression, we fit separate line segments to intervals of independent variables. Formally stating, independent linear models are assigned to individual partitions of feature spaces. This is pretty useful in the cases when the data assumes different linear relationships in separate intervals of the feature values. Generally, applying linear regression on such tasks can incur large statistical losses.  

It is important to note that despite it's better accuracy, it can be computationally inefficient because many independent linear regressions have to be performed.     

The points where the data is split into intervals are called **Break Points**. There are various statistical tests that are to be performed in order to determine the break points but the details of those tests are beyond the scope of this course.  

#### Useful Resources

* To get an overview of the concepts, go through **[this](https://storybydata.com/datacated-challenge/piecewise-linear-regression/)** article and **[this](https://en.wikipedia.org/wiki/Segmented_regression)** page.  

* Refer to the **[repo](https://github.com/srivatsan88/piecewise-regression/blob/master/piecewise_linear_regression.ipynb)** for a small demo on Piecewise Linear Regression.  

* (Optional) To delve deeper into the mathematical aspects and get hands on experience, go through **[this](https://www.fs.fed.us/rm/pubs/rmrs_gtr189.pdf)**. This is pretty complicated to understand and it is upto the interest of the reader.  

## Locally Weighted Regression

In Locally Weighted Regression, we try to fit a line locally to the point of prediction. What it means is that we give more emphasis to the training data points that are close to the point where prediction is to be made. A weight function (generally a bell shaped function) is used to determine the amount of emphasis given to a data point for prediction. This kind of model comes under **Non Parametric Learning** unlike the **Parametric Learning** models that we have seen so far. 

Such models are useful when the training data is small and has small number of features. It is computationally inefficient because a linear regression is performed everytime we need to predict some value. But at the same time, this allows us to fit even complicated non-linear curves with ease.  

#### Useful Resources

* Follow this article to get an [overview](https://medium.com/100-days-of-algorithms/day-97-locally-weighted-regression-c9cfaff087fb) of this model.

For classification tasks we need a different architecture. In the next section, we discuss about Logistic Regression - a regression tool employed for classification. 

## Logistic Regression

Logistic regression is a classifier that uses regression to obtain the probability of the input data belonging to one of various classes. Unlike Linear Regression, where the target values are continuous real valued, the target variables here are drawn from a finite set of discrete values. Formulation of logistic regression can be made where the parameters are estimated using gradient descent.  

* This **[article](https://towardsdatascience.com/logistic-regression-detailed-overview-46c4da4303bc)** covers the major aspects of Logistic Regression and should give you a firm grasp on the mathematics behind this algorithm

### Binary Logistic Regression

Binary logistic regression is used for classififcation into only 2 classes. Checkout **[this](https://www.statisticssolutions.com/binary-logistic-regression/)** short read on Binary Logistic Regression. 
<br>The output of a binary logistic classifier is a probability value between 0 and 1, where 0 and 1 represent the two classes. By now you must be familiar with activation functions. The activation function used for Logistic Regression is the Sigmoid Function, which is also known as the Logistic Activation function. You can read more about it **[here](https://towardsdatascience.com/activation-functions-neural-networks-1cbd9f8d91d6)**. 

### Multinomial Logistic Regression

Logistic regression can be binary or multinomial in nature. The **multinomial logistic regression** is also termed as **Softmax Regression**. 
* Go through this **[article](https://stats.idre.ucla.edu/stata/dae/multinomiallogistic-regression/)** to go deeper into the concepts of Multinomial Logistic Regression. 

The activation function used in the case of Multinomial Logistic Regression is known as the Softmax Activation Function. 

* Checkout this great **[article](https://medium.com/data-science-bootcamp/understand-the-softmax-function-in-minutes-f3a59641e86d)** on Softmax basics. 

Basically, the softmax function takes in a vector of real values as input, and generates a probability vector as the output. The dimension of this vector is the same as the number of classes for classification, and hence a single vector element having higher value than the rest of the vector elements helps us to classify the input vector (representative of an image, text, etc.) into a class. 

## Naive Bayes Classifier
Naive Bayes classifiers refer to a set of classification algorithms that share one underlying assumption, every pair of features being classified is independent of the other.

Let's understand what this means. Generally we would like to classify an n dimensional vector of input variables (can be discrete or continuous) into one of various classes. We can imagine this vector to represent our binary input data for instance where each element of the vector is a boolean. The Naive Bayes algorithms assume that the probability of one of those input variables (say the kth element of the vector) equaling a particular value, is independent of the value of the other input variables.

This may not seem very useful but what this does is it immensely reduces the training space as now we can train for each input feature independently. This allows us to feasibly set up a classifier based on Bayes rule.

#### Useful Resources

* This **[article](https://www.geeksforgeeks.org/naive-bayes-classifiers/)** will walk you through a solved example of applying the Naive Bayes algorithm for predictive & classification tasks. Towards the end, it also has code for implementing the Naive Bayes classifier available in```sklearn``` for the ''Iris dataset''.
* Implementing algorithms from scratch is a good way to consolidate your understanding about various specifics of the algorithm. Here is a **[tutorial](https://chrisalbon.com/machine_learning/naive_bayes/naive_bayes_classifier_from_scratch/)** to help you implement a Naive Bayes classifier from scratch in Python by creating your very own toy dataset. Once you are familiar, you could extent this to more complex datasets.
 
## Exploratory Data Analysis

Last week, we learned about Data Visualisation and Exploration. To get hands on experience on Data Analysis on Regression and Classification, refer to the links below - 
* **[Regression](https://github.com/MicrosoftLearning/Principles-of-Machine-Learning-Python/blob/master/Module2/VisualizingDataForRegression.ipynb)**
* **[Classification](https://github.com/MicrosoftLearning/Principles-of-Machine-Learning-Python/blob/master/Module2/VisualizingDataForClassification.ipynb)**

Now finally let us look into one important aspect of data analysis that is important for machine learning, data cleaning.

## Data Pre-Processing

Let us consider a simple classification problem using logistic regression. Suppose you have 10 columns in your data which would make up the raw features given to you. A naive model would involve training your classifier using all these columns as features. However are all the features equally relevant? This may not be the case. As a worst case example suppose all the data entries in your training set have the same value. Then it does not make sense to consider this as a feature since any tweaking to the parameter corresponding to this feature that you do can be done by changing the bias term as well. This is a redundant input feature that you should remove. Similarly if you have a column that has very low variance it may make sense to remove this feature from your dataset as well. When we work with high dimensional data sometimes it makes sense to work with fewer dimensions. Thus it makes sense to remove the lower variance dimensions. Note that sometimes this reduction of dimension may not be as straightforward and next week we will see how to do this using PCA.

* This **[article](https://machinelearningmastery.com/basic-data-cleaning-for-machine-learning/)** provides a proper introduction to data cleaning for machine learning
* This **[article](https://www.dataquest.io/blog/machine-learning-preparing-data/)** is also useful for data cleaning.

Another way we can clean and improve our data is by performing appropriate transformations on the data. Consider the task of Sentiment Classification using Logistic Regression. You are given a tweet and you have to state whether it expresses happy or sad sentiment. You could just take the tweet in and feed it into the classifier (using a particular representation, the details aren't important). But do all the words really matter? 

Consider a sample tweet
```
#FollowFriday @France_Inte @PKuchly57 @Milipol_Paris for being top engaged members in my community this week :)
```
Clearly any tags in this tweet are irrelevant. Similarly symbols like '#' are also not needed. Thus we need to clean the input data to remove all this unnecesary information. Further in Natural Language Processing words like 'for', 'in' do not contribute to the sentiment and a proper classification would require us to remove this as well. All of this comes under data cleaning and preprocessing.

The preprocessed version of the above tweet would be:
```
['followfriday', 'top', 'engag', 'member', 'commun', 'week', ':)']
```

* This **[article](https://towardsdatascience.com/data-preprocessing-concepts-fa946d11c825)** explains data preprocessing.
* This **[tutorial](https://towardsdatascience.com/twitter-sentiment-analysis-classification-using-nltk-python-fa912578614c)** uses Naive Bayes to solve the above tweet classification problem. Please go through this to acquaint yourself with the various data processing methods needed for natural language processing (Note that this tutorial uses sklearn to implement naive bayes instead of doing it from scratch. Feel free to skip the implementational details if you are facing issues with it as we will not be covering sklearn in this course)

The concepts of feature aggregration, data cleaning, dimensionality reduction are important for a data scientist and it is essential to have a proper understanding of them before continuing.  

## Generalised Linear Models

On a very high level, Generalised Linear Models (GLM) are a superclass of all linear models including Linear and Logistic Regression that we talked about earlier. 

* Linear Regression is based on the assumption that the data assumes **Gaussian/Normal Distribution**.
* Binary Logistic Regression is based on the assumption that data assumes **Bernoulli Distribution**.

GLM's are based on Exponential Family Functions. **[Exponential Family](https://en.wikipedia.org/wiki/Exponential_family)** includes these two and a lot of other distributions of data that we talked about in week 1. So therefore GLM's serve as a generalisation of all linear models. To get a firm hold on generalised linear models, head **[here](https://towardsdatascience.com/generalized-linear-models-9cbf848bb8ab)**.

---

Next week we will be looking at more supervised machine learning techniques. Till then stay safe and have fun.
