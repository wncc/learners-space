# Welcome to Week 3 of LS Python! 
This week we will be mainly covering Object Oriented Programming, specifically you will be learning the following topics: 
 * [Classes and Objects](#classes-and-objects) 
 * [Constructors and Destructors in Python](#constructors-and-destructors)
 * [Access Modifiers](#access-modifiers-in-python)
 * [Inheritance in Python](#inheritance)
 * [Encapsulation](#encapsulation)
 * [Overloading](#function-overloading-and-polymorphism)
 * [Polymorphism](#function-overloading-and-polymorphism)

## Introduction to Object Oriented Programming 
As the name suggests, Object-Oriented Programming or OOPs refers to languages that uses objects in programming. Object-oriented programming aims to implement real-world entities like inheritance, polymorphism etc in programming. The main aim of OOP is to bind together the data and the functions that operate on them so that no other part of the code can access this data except that function.

Head over to this link for a brief introduction on each of the topics listed above - **[Python OOP](https://www.programiz.com/python-programming/object-oriented-programming)** 

Now lets discuss each of the topics in detail - 

## Classes and Objects 
A class is a user defined blueprint or prototype from which objects are created. It represents the set of properties or **methods** that are common to all objects of one type. You can think of a class as a collection of many different functions and attributes (variables) that can be accessed by an object of that class. These methods inside a class are defined almost in the same way normal Python functions are defined, with a major difference being the 'self' argument and some special methods only found in a class body, for example:- the **'\_init_'** method, **'\_add_'** method, etc. 

An Object is a basic unit of Object Oriented Programming and a way to represent the classes you have declared in your program. And thus an object can also be sometimes called an instance of a class. Whenever you create an object of a class, you can access all the methods which you have declared in the body of the class. (Note that this is not possible in the case of Private classes (covered later)). 

You can check out any one of these detailed tutorials on Classes and Objects in Python based on your preference -
* **[Python Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)**
* **[Python Classes and Objects Detailed](https://www.programiz.com/python-programming/class)**
* Detailed Video Tutorials on Classes and Objects - **[Video #1](https://www.youtube.com/watch?v=v_Jp11xqCzg&list=PLzMcBGfZo4-l1MqB1zoYfqzlj_HH-ZzXt&index=2&t=0s)** and **[Video #2](https://www.youtube.com/watch?v=jQiUOV15IRI&list=PLzMcBGfZo4-l1MqB1zoYfqzlj_HH-ZzXt&index=2)** 

### Constructors and Destructors 
The special methods found in a class are related to another concept in OOP, known as Constructors and Destructors. A Constructor is a special function which is **automatically** called whenever a class object is created. Similarly, a Destructor is a special function which is automatically executed whenever a class object is destroyed, i.e, goes out of scope. By now you must know what the 'scope' of a variable means. 
<br> A constructor is unique to a class, and is represented using the **'\_init_'** method in a class. Similarly, a destructor is represented using the **'\_del_'** method in the class. 
* For more information, check out this video on - **[Constructors and Destructors](https://www.youtube.com/watch?v=NSssW0duUkQ)**

### Access modifiers in Python
In Python (and other OOP languages), we can restrict the amount of **access** to the methods and attributes of a class given to the object of the classes. This technique is particularly helpful when we are inheriting a class from another parent class (don't worry, inheritance is covered later) and when we declare an object of the child class, we want the object to access only certain attributes and methods of the parent class. There are three types of Access Modifiers in Python: **Public, Private** and **Protected.**

Refer to these links for a better understanding on Access Modifiers:
* **[Access Modifiers in Python](https://www.geeksforgeeks.org/access-modifiers-in-python-public-private-and-protected/)**
* **[Video Tutorial on Public and Private classes in Python](https://www.youtube.com/watch?v=xY__sjI5yVU&list=PLzMcBGfZo4-l1MqB1zoYfqzlj_HH-ZzXt&index=7&t=0s)**

## Inheritance
Inheritance in OOP is a property that allows us to define a class that inherits all the methods and attributes from another class.
Parent class is the class being inherited from, also called base class. Child class is the class that inherits from another class, also called derived class. So now you know what I meant earlier in Access Modifiers. 
* Refer to this link for learning more about Inheritance in Python - **[Inheritance](https://www.programiz.com/python-programming/inheritance)** (Also checkout further links in the same page)
* To learn using a video, refer to this link - **[Inheritance Video](https://www.youtube.com/watch?v=H2SQrZK2nvM&list=PLzMcBGfZo4-l1MqB1zoYfqzlj_HH-ZzXt&index=4&t=0s)**

When we talk about Inheritance, many other rules and details come along with it. For example try to answer the following questions:
- What happens when you create an object of a child class, and try to call a method in the child class which has the same name as the another method in the parent class, which method is called?
- What all methods and attributes are carried over from the parent class to the child class? And how does that change with the access modifier used in the parent class?
These questions are answered using the concepts described below:
### Encapsulation
Encapsulation is a very useful tool when it comes to preventing access to some part of data that may be private, or an useful element of the program which should not be modified. This is done using the 'Access Modifier' that we learnt earlier, by making some methods and attributes of the parent class 'Private', so that an object of the child class is not able to access them. 
* Read more about encapsulation from here - **[Encapsulation in Python](https://www.geeksforgeeks.org/encapsulation-in-python/)**
* You can also watch a video on this if you don't like to read - **[Encapsulation Video](https://www.youtube.com/watch?v=TFLo9m0jFEg)**

As you can see, there are many nuances involved with Inheritance, so make sure that you give this section enough time till you understand each and every rule. 
It may seem confusing in the beginning, but if you just keep going at it, its not that difficult. 

### Function Overloading and Polymorphism 
There is a complication which can arise when we are working with functions, known as Overloading. The complication is as follows; what if I define two functions with the same name, but different arguments or different return datatype (I hope you know what these terms mean) and I want to access each of them individually?
And Polymorphism is similar to Function overloading with the basic difference being that Polymorphism is generally assosciated with classes and Inheritance, where the ambiguity arises when a class object tries to access those methods. 
<br> There are many other complications assosciated with Overloading and Polymorphism, so it is important you know about this. 
* Read more about it from here - **[Polymorphism](https://www.geeksforgeeks.org/polymorphism-in-python/)**
* Watch this amazing video on **[Function Overloading](https://www.youtube.com/watch?v=39m3rstTN8w&list=PLzMcBGfZo4-l1MqB1zoYfqzlj_HH-ZzXt&index=5&t=0s)** which also talks about the other special functions in classes (apart from Constructors and Destructors), that I talked to you about earlier (**\_sub_, \_add_**, etc.)
* You can also consider this short read on overloading - **[Method Overloading](https://www.geeksforgeeks.org/python-method-overloading/)**


## Assignment 3 
Please refer to the **[Week 3 Assignment Notebook](./Week3_Assignment.ipynb)** for this week's assignment. 

### Instructions to download the assignments:
1. Open on the respective `.ipynb` file on GitHub
2. In the upper right corner, there are several buttons and icons including the ones shown below. Click on the Raw Button.
       Raw | Blame
      --- | ---
      
3. The python notebook opens as raw text in browser. Right click->Save as OR just press CTRL + S. Save the notebook, open it using Jupyter Notebook you just installed and start learning! 


If you get stuck in any of the above questions, feel free to post them in the [Telegram](https://t.me/joinchat/OEr2Tk_ieMMmwihkBQVjFw) group. Additionally, you can also search for the problems online. Another aspect to becoming a good programmer is learning how to debug your code! it is very common to encounter error along the way of programming and in that case, try reading the error and understanding the reason behind it. More often than not, you may not be able to figure out yourself, the cause of the error. So, in that case, copy the error meassage and google it! You would be surprised how common such practices are and there are many forums where people may have already asked similar questions and have gotten solutions too! Stack Overflow is one such question and answer site for professional and enthusiast programmers. 

Congratulations! You have successfully completed Week 3 of Python! Keep up the enthusiasm! 

Again, if you are having any difficulties with the course, please reach out to one of the moderators and we will surely help you out. 
<br>See you in Week 4!








