# Machine Learning (Learner's Space 2020)

Hello everyone, Welcome to the Machine learning course offered by WnCC in association with Career Cell under Learner's Space. 

In this course, we cover the essentials of Classical Machine Learning or the Pre-Deep Learning era. The readers are then introduced to Deep Learning - the backbone of Artifical Intelligence today. This course requires one to be familiar with basics of Python and some background in Calculus. 

Following is the weekly course structure - 

 * **Week 1: [Brushing up the Basics](https://github.com/wncc/learners-space/tree/master/Machine%20Learning/Week%201)**
 * **Week 2: [Linear Models](https://github.com/wncc/learners-space/tree/master/Machine%20Learning/Week%202)**
 * **Week 3: [Unparametrised Learning & Unsupervised Learning](https://github.com/wncc/learners-space/tree/master/Machine%20Learning/Week%202)**
 * **Week 4: [Introduction to Neural Networks](https://github.com/wncc/learners-space/tree/master/Machine%20Learning/Week%204)**
 * **[Mid-course Evaluation](./MId%20Term%20Assignment/README.md)**
 * **Week 5: [Applying Neural Networks](https://github.com/wncc/learners-space/tree/master/Machine%20Learning/Week%205)**
 * **Week 6: [Deep Learning Models in Practice](https://github.com/wncc/learners-space/tree/master/Machine%20Learning/Week%206)**
 * **Week 7: [End Course Evaluation](./End%20Term%20Assignment/README.md)**
 
---

# Why This Course?

You must be wondering, *"Not again! Why this course? Why should I even bother about this course when there are hundreds of other courses and tutorials available over the internet"*

It is rightly said *"Googling is an art"* and believe me it is not easy to Google things. Now, one can say that what a big deal, just type out the topic on Google Search Bar and *"Woah! A million results!"*. It is great that you have a million results at your disposal but with a million results creeps in a great challenge - **Quality**. There are tens of thousands of resources available to learn Machine Learning over the internet. But not every resource is good enough to give you insights into the concepts and help you gain intuition as to why things are working. There are even resources that give you wrong information. 

We also had a similar experience when we were trying to learn Machine Learning. So, we thought of making this course unique and easy for the reader to follow. We don't give complete analysis of concepts or every small bit of detail, rather we link up the best resources on that topic over the internet for your reference. The references are so well written that going through them will essentially clear every bit of doubt that you might have in that topic and make your undertanding crystal clear.  

So in essence, we have done the Herculean Task of Googling for you and we present you this course where we give brief description about stuff and link up best resources over the internet to bring out the master of Data Science inside you. Happy Learning! 

# Structure of the Course

## Week 1
 
We begin our journey in the world of Machine Learning by laying down the foundation stone of various associated domains of Mathematics and Coding skills. 

* We start with **Python**, probably one of the most popular languages around the globe used in Machine Learning and programming at large. 
* We then head on to one of the most important skills of Machine Learning namely **Data Plotting and Visualisation**. It is one of the first steps to solve a machine learning challenge. Unless one is familiar with the data he/she will deal with is essential to developing a good Machine Learning model for the task. 
* We talk about **Data Distribution** which is central to understanding the kind of model that can be used to solve the problem at hand.
* Let us say, we know what data we want to deal with and know about it's distribution but we generally can't feed the data directly to our model and hence it is essential to **prepare** the data and **pre-process** it as per need of our model. So, we look at a really useful library called Pandas.
* Having prepared the data, now the question is, how to process it efficiently. Here creeps in **Numpy - Numerical Python**. One of the most extensively used libaries for computing and widely used to speed up the task at hand.
* We now try to acclimatise readers with Machine Learning foundations namely, **Calculus and Linear Algebra**.

We are now set to dive deep into Machine learning and every aspect of it in detail starting with week 2.
 
## Week 2

We begin our walk with basics of Machine Learning i.e. Regression and Classification in this week.

* **Linear Regression** is probably one of the most fundamental ideas in Machine Learning and in fact, Machine Learning build around Linear Regression.
* A more efficient model than simple Linear Regression finds it's way onto the middle often referred to as **Segmented Regression**. We talk about the relative performance of this model wrt Simple Linear Regression. 
* A really good Linear Regression model based on really good observations is **Locally Weighted Regression**, which we talk in detail about.
* From the world of linearity in regression model, we jump into **Logistic Regression for Classification of Data**.
* We talk about a relatively advanced model called **Naive Bayes Classifier** which was used extensively in Machine Learning era.
* We then try to build upon the Data Analysis we learned in Week 1 by understanding **Exploratory Data Analysis** and **Data Pre-Processing**.
* We finally try to unify all the types of linear models under one umbrella called **Generalised Linear Models (GLM)**. This topic turns to be math intensive and so we in some sense try to make it as much as intutive as possible and avoided the math behind stuff.


## Week 3

From the realm of Linear Models, we try to explore some non-linear models in this week and understand some **Unsupervised Learning** models.

* We start with a non-parametric learning model called the **Decision Tree**. This is a really simple idea and the first glance may seem to be trivial but is a really powerful model for both **Regression** and **Classification**. It is really important to understand this well as this was used and is still in use extensively.
* We also talk about an Algorithm for construcyion of Decision Trees.
* We then talk about **Ensemble**. We talk about an ensemble of **Decision Trees** known as **Random Forest** and try to figure out the ways in which we should try to ensemble decision trees. We talk about pros and cons of this model relative to Decision Trees.
* How should we deal an image that has hundreds of dimension. Is it feasible to use the entire image in its original form in our conventional models? To answer such questions, we try to explain a technique called **Principal Component Analysis** that is used greatly for **Face Recognition**. This in essence is a **Dimensionality Reduction Technique**.
* We now, jump to an **Unsupervised Learning** model named **k Nearest Neighbours (kNN)** used to make some sense of the data by clustering the data. It is used widely today as a Classifier. It is essentially a **Non Parametric Learning** model.

## Week 4

This week we take a flavour of **Neural Networks** that have revolutionised the field of Artifical Intelligence. It is used extensively in almost every domain of Artifical Learning. With it's advent, the conventional learning models lost their importance because in some sense this unifies everything into one and only one model that can do almost everything that the machine learning models do. 

* We talk about the fundamentals of **Neural Nets** and the associated mathematics for a better understanding of it's working.
* We also talk about few general concepts like **Loss Function** and **Optimisation techniques**.
* From this week onwards, we also start to look at **practical aspects** of Machine Learning models which are undoubtedly the determiners of efficiency of a model. They are crucial things to which one must arrive at before diving into to solving the task at hand.
* We also introduce some **statistical** concepts that are closely related to Machine Learning and are fundamental to the understanding of Machine learning models.
* We also give a few practice exercises to get your understanding clear on this really important model.

## Week 5

This week, we start with implementation details of Neural Networks in Standard Libraries like Tensorflow and Keras. We also try to further our knowledge of Neural Nets with more advanced concepts.

* We start with tutorials on **tensorflow** and **Keras** where we learn about the implementation of Neural Nets and applying them to tasks.
* We then head on to Convolutional Neural Nets. Probaby one of the greatest developments in the field of Deep Learning that has indeed changed the field of Computer Vision completely. 
* We talk a lot of detail about CNN's and introduce you to **Conv Layers** and **Pooling Layers**.
* A few exercises have been given to acquaint readers with Neural Nets and Convolutional Neural Nets.

## Week 6

In this week, we talk a lot about practical details of Neural Nets and how they are crucial in determining the performance of our models.

* We start with **Initialisation of Parameters** and talk extensively of it's effect on learning process of a model.
* We try to unify all the techniques into one standard expression of Standard Deviation as explained in a Research Paper added in the content section.
* We head on to essentially our last topic of discussion i.e. **Dropouts**. Google came up with this wonderful idea of Dropouts that in some sense allowed an ensemble using a single neural net and this improved performance greatly.

## Week 7

In this final week, we give a well thought assignemnt to the readers so that they can get try their hands on a problem using all the concepts that they have learnt throughout the course. This assignment is also used to judge and evaluate the performance of the student based on how well the code is written and the accuracy of the model. 

This assignment is based on Neural Networks that was first designed some 70 years back by Frank RosenBalt. Neural networks form the backbone of the entire Artifical Intelligence Industry today. Deep Learning has really taken off recently and through this assignment we try to give you a flavour of the Deep Learning domain through a very basic exercise. 

---

# Some Really Useful Resources

* **[Towards Data Science](https://towardsdatascience.com/):** Probably, one of the most frequently used website by Data Scientists in general. It contains millions of articles written by a multitude of personalities ranging from students like you, to professional Data Scientists. 
* **[Stanford CS 229](https://www.youtube.com/watch?v=jGwO_UgTS7I&list=PLoROMvodv4rMiGQp3WXShtMGgzqpfVfbU) :** This course by the AI Guru Andrew Ng at Stanford is great for advanced content in Machine Learning. It contains a lot of rigour behind stuff and is a one stop course for Mathematics behind Machine Learning.  


With this we come to the end of our course that was developed completely by the members of the **WnCC  Family** with great efforts and an ambition to give the reader a tour of the really amazing Machine Learning field and acquaint you with the potential of Machine Learning to revolutionise the era of technology and make this world even more exciting.
 
<p align="center">Created with :heart: by <a href="https://www.wncc-iitb.org/">WnCC</a></p>

