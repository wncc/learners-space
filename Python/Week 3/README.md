# Welcome to Week 3 of LS Python! 
This week we will be mainly covering Object Oriented Programming, specifically you will be learning the following topics: 
 * Classes and Objects 
 * Methods
 * Constructors and Destructors in Python
 * Inheritance in Python
 * Encapsulation
 * Polymorphism 

## Introduction to Object Oriented Programming 
As the name suggests, Object-Oriented Programming or OOPs refers to languages that uses objects in programming. Object-oriented programming aims to implement real-world entities like inheritance, polymorphism etc in programming. The main aim of OOP is to bind together the data and the functions that operate on them so that no other part of the code can access this data except that function.

Head over to this link for a brief introduction on each of the topics listed above - **[Python OOP](https://www.programiz.com/python-programming/object-oriented-programming)** 

Now lets discuss each of the topics in detail - 

## Classes and Objects 
A class is a user defined blueprint or prototype from which objects are created. It represents the set of properties or **methods** that are common to all objects of one type. You can think of a class as a collection of many different functions and attributes (variables) that can be accessed by an object of that class. These methods inside a class are defined almost in the same way normal Python functions are defined, with a major difference being the 'self' argument and some special methods only found in a class body, for example:- the '__init__' method, '__add__' method, etc. 

An Object is a basic unit of Object Oriented Programming and a way to represent the classes you have declared in your program. And thus an object can also be sometimes called an instance of a class. Whenever you create an object of a class, you can access all the methods which you have declared in the body of the class. (Note that this is not possible in the case of Private classes (covered later)). 

You can check out any one of these detailed tutorials on Classes and Objects in Python based on your preference -
* **[Python Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)**
* **[Python Classes and Objects Detailed](https://www.programiz.com/python-programming/class)**
* Detailed Video Tutorials on Classes and Objects - **[Video #1](https://www.youtube.com/watch?v=v_Jp11xqCzg&list=PLzMcBGfZo4-l1MqB1zoYfqzlj_HH-ZzXt&index=2&t=0s)** and **[Video #2](https://www.youtube.com/watch?v=jQiUOV15IRI&list=PLzMcBGfZo4-l1MqB1zoYfqzlj_HH-ZzXt&index=2)** 

### Access modifiers in Python
In Python (and other OOP languages), we can restrict the amount of **access** to the methods and attributes of a class given to the object of the classes. This technique is particularly helpful when we are inheriting a class from another parent class (don't worry, inheritance is covered later) and when we declare an object of the child class, we want the object to access only certain attributes and methods of the parent class. There are three types of Access Modifiers in Python: **Public, Private** and **Protected.**

Refer to these links for a better understanding on Access Modifiers:
* **[Access Modifiers in Python](https://www.geeksforgeeks.org/access-modifiers-in-python-public-private-and-protected/)**
* **[Video Tutorial on Public and Private classes in Python](https://www.youtube.com/watch?v=xY__sjI5yVU&list=PLzMcBGfZo4-l1MqB1zoYfqzlj_HH-ZzXt&index=7&t=0s)**

## Inheritance
