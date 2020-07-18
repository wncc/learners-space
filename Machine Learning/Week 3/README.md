# Week 3

Welcome to Week 3! This week we will be covering many powerful classical machine learning algorithms before moving onto modern (aka deep learning) algorithms next week.

We'll begin with a model that appears rather simple at first, Decision Tree. However this is an incredibly powerful model that relies a lot on information theory and entropy (remember thermodynamics anyone?) and we will discuss some of the fundamentals behind this (although I myself am not an expert on this and most of the advanced ideas are beyond the scope of this course). Then we will look at an extension of this model called Random Forest and then we will consider an important data dimensionality reduction technique called PCA and we end it by talking about kth nearest neighbours.

So let's get started we have a busy week ahead of us!

## Decision Trees

Let's forget about machine learning for some time and focus on you. You are trying to learn machine learning through this course. It's probably due to a lot of decisions that you ended up here. And it was always a sequence of decisions. When you decided to wake up early (or late) you made a decision. Then you decided to study. Then you decided to study machine learning.

Indeed all a decision tree tries to do is create a sequence of decisions that would result in the machine learning algorithm come to an outcome. As an extremely simple example consider a machine learning algorithm that classifies all points in the xy plane to the right of the y axis as positive and others as negative.

Then the decision tree is a very simple one here, the algorithm will check if `x>0` and then label positive else it would label negative. However rarely will the decision tree be this simple.

This **[link](https://heartbeat.fritz.ai/introduction-to-decision-tree-learning-cd604f85e236)** provides an introduction to decision trees (please read only the beginning part without going into construction).

All this may seem very simple to you but one question remains. How will the algorithm construct this tree? Clearly figuring out what questions to ask is far from simple. Note that we only ask questions related to the features given to us in the dataset and use these questions to come to a conclusion. Note that although decision trees can be used for both regression and classfication we only consider classification here. So our aim is to come up with a set of questions that will allow us to classify a dataset into labels.

### Constructing Decision Trees

Basically we will use recursion. Observe that every point when you (aka the algorithm) ask any question the dataset splits. For instance consider the titanic dataset. You may ask one question regarding the age. If the age is `>= 30` go to the right half else go to the left half. Both the left and right half are themselves decision trees.

So what we can do is look for the locally most optimum question. That is the question that would result in most amount of information about the classes being conveyed. For instance if all people above the age of 30 survived the titanic disaster then this is a very good question to ask since all elements in the right half belong to the survived category and so we can terminate the right half immediately.

But how do we know which questions are best to ask? There are metrics for this and we investigate two of them namely information entropy and gini impurity.

#### Information Entropy

Remember thermodynamics? Yeah we all probably hated that chapter during JEE (I didn't but that's another story). The idea that entropy leads to disorder is not only a physical idea but also a mathematical one. Observe that we want after asking a question to split the dataset into halves such that each halves are as homogenous as possible (only then would your question be the most discriminating). But wait. That would mean the entropy increased since we are moving towards order! (Second law doesn't hold since this is not physics xD).

This gives us an idea. Ask those questions that increase the entropy the most! Or in other words we want to increase the information gain. How do we compute this entropy? We have to use information entropy for this.

* This **[link](https://www.kdnuggets.com/2020/01/decision-tree-algorithm-explained.html)** talks in brief about information entropy and you may go over it once.
* This **[wikipedia section](https://en.wikipedia.org/wiki/Decision_tree_learning#Information_gain)** talks in detail about the math behind decision tree learning.
* This **[article](https://www.geeksforgeeks.org/decision-tree-implementation-python/)** provides the code for using information gain based decision trees using sklearn.


#### Gini Impurity

Instead of looking at entropy we can look at another metric. Split the dataset with a question in such a way such that each of the split datasets are as pure as possible. Pure means homogenous. Although entropy was also doing the same thing we can use a simpler way at estimating this. This way is termed gini impurity.

Essentially Gini Impurity is a measurement of the likelihood of an incorrect classification of a new instance of a random variable, if that new instance were randomly classified according to the distribution of class labels from the data set.

This **[article](https://towardsdatascience.com/decision-tree-in-machine-learning-e380942a4c96)** uses Gini Impurity for creating decision trees. Please go through this to understand the mathematical formulation of gini impurity and the code as well.

That is all we want to cover in standalone Decision Trees. We will talk a bit more about them in pragmatics later on (overfitting).

## Random Forests

THe main idea behing using random forests is that maybe a single decision tree could be inaccurate. But what if we have 10 or 20 decision trees that are uncorrelated and working independently? Then our probability of getting the correct classification would skyrocket! And indeed a random forest is basically a collection of decision trees that achieves this.

* This **[article](https://towardsdatascience.com/understanding-random-forest-58381e0602d2)** covers random forests in theory.
* This **[article](https://towardsdatascience.com/random-forest-in-python-24d0893d51c0)** provides you with a step by step implementation in Python.

Now let's get onto PCA.

## Principle Component Analysis

The main idea of PCA is the following:

Suppose we have a highdimensional dataset of dimension `d` that we want to compress along `k` dimensions.
Given this high dimensional dataset retain the `k` dimensions along the eigenvectors of the covariance matrix of the data inputs with the highest eigenvalues (out of the total `d` eigenvectors (this is actually `d-1` after normalisation)). This compression will retain the maximum variance among all other compressions.

That probably made no sense. If you just implement this you are done with PCA. Finding covariance matrix and eigenvectors is pretty easy with numpy.

But don't do that yet. Let's understand why this works.

* This **[video](https://www.youtube.com/watch?v=TJdH6rPA-TI)** beautifully explains what PCA does.
* These **[notes](http://cs229.stanford.edu/notes/cs229-notes10.pdf)** by Andrew NG brilliantly explain the math behind PCA.
* This **[lecture](https://www.youtube.com/watch?v=rng04VJxUt4)** explains PCA in a simpler manner.
* (Optional) These CS663 IITB **[slides](https://www.cse.iitb.ac.in/~ajitvr/CS663_Fall2016/face_recognition.pdf)** explain how PCA is derived and a beautiful application of PCA for face recognition is given (bonus points to those who code this up!) 


That should be all for PCA. Let's talk about kNNs

## kth Nearest Neighbour

This is probably the simplest algorithm that we'll talk about today.

Suppose you want to classify data. You have a training set of `d` dimensions. What you can do is simply find the kth nearest points in the training set to any datapoint in your test set. Then simply return the label which appears the maximum times among these k labels.

Why would this work? Well because birds of a feather flock together! Assuming that there is indeed a proper boundary separting different classification regions you would hope that points belong to the same class are clustured together at different regions. Thus by looking at the class of the closest points you can get an estimate of which class your test point belongs to.

What should `k` be though? This is a hyperparameter that you should tweak! (Hyperparamter refers to variables that you tweak in your algorithm to get the best performance).

* This **[article](https://www.geeksforgeeks.org/k-nearest-neighbours/)** talks about kNNs in a simple manner.
* For more insight refer to this **[article](https://towardsdatascience.com/machine-learning-basics-with-the-k-nearest-neighbors-algorithm-6a6e71d01761)**.

We could end here but wait. How do you really find the kth nearest neighbours? You have to loop through all examples in your training set every time you want to evaluate your machine learning algorithm. This would be incredibly SLOW!

We could give up here but there is seemingly a way out of this. We use what is termed as locality sensitive hashing for kNNs. Note that this is a bit more advanced so go through it slowly.

* This **[article](https://towardsdatascience.com/fast-near-duplicate-image-search-using-locality-sensitive-hashing-d4c16058efcb)** talks about using LSH with kNNs for findind duplicate images. (Note this uses deep learning to encode images feel free to skip this and just go through how hashing is done to generate hyperplanes that are then used with kNNs).

* This **[video](https://www.youtube.com/watch?v=LqcwaW2YE_c)** also goes over kNNs with locality sensitive hashing.

You can also refer to this **[playlist](https://www.youtube.com/playlist?list=PLBv09BD7ez_48heon5Az-TsyoXVYOJtDZ)** to know more about kNNs.


That's it for this week! Stay tuned for the graded assignment that will be due by the end of this week! Have fun with the assignment and we hope to see you next week.
