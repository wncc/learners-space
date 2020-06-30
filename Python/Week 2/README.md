# Welcome to Week 2 of Learner Space's Python! 

For the second week we will be covering the following topics:

* Installation and setup of Anaconda 
* Python Functions
* Scope of Variables
* Recursion
* Python Modules and Packages
* Some Standard Libraries of Python
* Assignment for Week 2

So let's get started...

# Installation and Setup of Anaconda

Note: If you already have a python IDE like PyCharm or Spyder installed in your system, you may skip this section.

Anaconda is a free and open-source distribution of the Python and R programming languages for scientific computing (data science, machine learning applications, large-scale data processing, predictive analytics, etc.), that aims to simplify package management and deployment. The distribution includes data-science packages suitable for Windows, Linux, and macOS. It is developed and maintained by Anaconda, Inc., which was founded by Peter Wang and Travis Oliphant in 2012. As an Anaconda, Inc. product, it is also known as Anaconda Distribution or Anaconda Individual Edition, while other products from the company are Anaconda Team Edition and Anaconda Enterprise Edition, which are both not free.

Anaconda Navigator is a desktop graphical user interface (GUI) included in Anaconda distribution that allows users to launch applications and manage conda packages, environments and channels without using command-line commands. Navigator can search for packages on Anaconda Cloud or in a local Anaconda Repository, install them in an environment, run the packages and update them. It is available for Windows, macOS and Linux.

The following applications are available by default in Navigator:

* JupyterLab
* Jupyter Notebook
* QtConsole
* Spyder
* Glue
* Orange
* RStudio
* Visual Studio Code

Follow this [Installation Guide](https://docs.anaconda.com/anaconda/install/) to install Anaconda on your system. 

After Successful Installation you can open Anaconda and see the above mentioned applications. The 2 important applications of our interest are Jupyter Notebooks and Spyder.

Spyder is an open source cross-platform integrated development environment (IDE) for scientific programming in the Python language. Spyder integrates with a number of prominent packages in the scientific Python stack, including NumPy, SciPy, Matplotlib, pandas as well as other open source software. It is released under the MIT license.

### Why a Python IDE ?

Jupyter Notebooks have tons of Advantages. It is user-friendly, easy to debug and you can make a single change immedietly to a small chunk of code and see the effect. It is ideal for experimentation and prototyping. Once the experimentation and prototyping is done, you usually need to move the model/analysis ‘to production’, which is essentially software development and should result in scalable, maintainable, robust code. You simply don’t want do this with a notebook, but develop a properly structured set of source files with an IDE like Spyder or PyCharm that supports things like version control, linters, running automated tests etc. 

You may use Jupyter Notebooks for most part of the tutorial but for modules/packages section it is prefferred to use Spyder to make .py files for a better understanding of the topic.

 <hr>
 
As you are familiar with Jupyter Notebooks now, in this tutorial, most part of the tutorial, that is definitions and code snippets have been covered in the notebooks for a better understanding of the topic. 

# Python Functions

A function is a set of statements that take inputs, do some specific computation and produces output. The idea is to put some commonly or repeatedly done task together and make a function, so that instead of writing the same code again and again for different inputs, we can call the function.

This [Notebook](https://github.com/abhipaiangle/learners-space/blob/master/Python/Week%202/Notebook1.ipynb) covers the most aspects of Python Functions. Download the Notebook and make changes to the code and see how they reflect in the output.

If you want to read more on functions, you can have a look at [this](https://www.geeksforgeeks.org/functions-in-python/) and [this](https://automatetheboringstuff.com/2e/chapter3/)

If you prefer watching a video tutorial, watch this [Youtube PLaylist's](https://www.youtube.com/playlist?list=PLzMcBGfZo4-mFu00qxl0a67RhjjZj3jXm) #12 Tutorial.

### Scope of a Variable

Scope refers to the visibility of variables. In other words, which parts of your program can see or use it. Variables that are defined inside a function body have a local scope, and those defined outside have a global scope. This means that local variables can be accessed only inside the function in which they are declared, whereas global variables can be accessed throughout the program body by all functions

### Recursion

The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. Using recursive algorithm, certain problems can be solved quite easily.

Check this [Notebook](https://github.com/abhipaiangle/learners-space/blob/master/Python/Week%202/Notebook2.ipynb) for learning about Scope and Recursion



Great! Now that you have learnt about funtions and scopes in Python, let's move on to the next section.
<hr>

# Python Modules and Packages

This [Notebook](https://github.com/abhipaiangle/learners-space/blob/master/Python/Week%202/Notebook3.ipynb) covers most aspects of Python Modules and Packages. You may use Spyder/PyCharm for this but if you are using Google Colab, read the instructions given in the notebook.

To read more about Modules and Packages head over to [this](https://www.geeksforgeeks.org/python-modules/) and [this](https://www.learnpython.org/en/Modules_and_Packages)


# Some Standard Libraries of Python

In python, collection of predefined modules and packages is called a library. Here, we will learn about some of the standard library modules.

* **math** - The math module is used to access mathematical functions in the Python. All methods of this functions are used for integer or real type objects, not for complex numbers. Refer [this](https://docs.python.org/3/library/math.html) documentation for learning different functions of math.

* **random** - This module implements pseudo-random number generators for various distributions. Refer [this](https://docs.python.org/3/library/random.html) documentation of random module.

* **time** - This module provides various time-related functions. Refer [this](https://docs.python.org/3/library/time.html) documentation of time module.

* **datetime** - The datetime module supplies classes for manipulating dates and times. Refer [this](https://docs.python.org/3/library/datetime.html) documentation of time module.

* **re** - This module provides regular expression matching operations similar to those found in Perl. Refer [this](https://docs.python.org/3/library/re.html) documentation of re module.

<hr>

# Learning with Hands-on code

Here are some problems for you to practise:

* [The Block Game](https://www.codechef.com/problems/PALL01)

* [Cop and the Thief](https://www.codechef.com/problems/COPS)

### Assignment - Week 2

* [Assignment 2](https://github.com/abhipaiangle/learners-space/blob/master/Python/Week%202/Week2_Assignment.ipynb)

This Assignment contains 4 Questions. With the content provided in the tutorial, we assume you will be able to solve these problems with ease. Good Luck!!

<br> The Assignment 2 notebook will be used for evaluation of the course, hence you are expected to complete them within the week.

### Instructions to download the assignments:
1. Open on the respective `.ipynb` file on GitHub
2. In the upper right corner, there are several buttons and icons including the ones shown below. Click on the Raw Button.
       Raw | Blame
      --- | ---
      
3. The python notebook opens as raw text in browser. Right click->Save as OR just press CTRL + S. Save the notebook, open it using Jupyter Notebook you just installed and start learning! 


If you get stuck in any of the above questions, feel free to post them in the [Telegram](https://t.me/joinchat/OEr2Tk_ieMMmwihkBQVjFw) group. Additionally, you can also search for the problems online. Another aspect to becoming a good programmer is learning how to debug your code! it is very common to encounter error along the way of programming and in that case, try reading the error and understanding the reason behind it. More often than not, you may not be able to figure out yourself, the cause of the error. So, in that case, copy the error meassage and google it! You would be surprised how common such practices are and there are many forums where people may have already asked similar questions and have gotten solutions too! Stack Overflow is one such question and answer site for professional and enthusiast programmers. 

For codechef questions, you can also search for the problems online with their name and problem code and most of the times you will easily find a solution for it. 

Congratualtions! You have successfully completed Week 2 of Python! Keep up the enthusiasm! 

Again, if you are having any difficulties with the course, please reach out to one of the moderators and we will surely help you out. 
<br>See you in Week 3!

<hr>













