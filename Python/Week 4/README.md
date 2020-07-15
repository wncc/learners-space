# Welcome to Week 4 of Learner Space's Python! 

We are extremely glad that you have been constantly keeping up the enthusiasm and following the course religiously. For the fourth week we will be covering the following topics:
* Exception Handling
* Iterators
* Generators
* Virtual Environment (important)

<hr>

### Exception Handling

Error in Python can be of two types i.e. Syntax errors and Exceptions. Errors are the problems in a program due to which the program will stop the execution. On the other hand, exceptions are raised when some internal events occur which changes the normal flow of the program.

Head over to this [Notebook](https://github.com/abhipaiangle/learners-space/blob/master/Python/Week%204/Notebook1.ipynb) to learn about Python Exceptions.

To read more about Exception Handling refer [this](https://www.geeksforgeeks.org/python-exception-handling/)

### Iterators

Iterator in python is any python type that can be used with a ‘for in loop’. Python lists, tuples, dicts and sets are all examples of inbuilt iterators. These types are iterators because they implement following methods.In fact, any object that wants to be an iterator must implement following methods.

__ iter__ method that is called on initialization of an iterator. This should return an object that has a next or 
__ next__ (in Python 3) method.

next ( __ next__ in Python 3) The iterator next method should return the next value for the iterable. When an iterator is used with a ‘for in’ loop, the for loop implicitly calls next() on the iterator object. This method should raise a StopIteration to signal the end of the iteration.

Check out this [Notebook](https://github.com/abhipaiangle/learners-space/blob/master/Python/Week%204/Notebook2.ipynb) to learn about Python Iterators.

To read more about Iterators refer [this](https://www.geeksforgeeks.org/iterators-in-python/)

### Generators

A generator-function is defined like a normal function, but whenever it needs to generate a value, it does so with the yield keyword rather than return. If the body of a def contains yield, the function automatically becomes a generator function.

Check out this [Notebook](https://github.com/abhipaiangle/learners-space/blob/master/Python/Week%204/Notebook3.ipynb) to learn about Python Generators.

To read more about Generators refer [this](https://www.geeksforgeeks.org/generators-in-python/)

# Virtual Environment 

A virtual environment is a tool that helps to keep dependencies required by different projects separate by creating isolated python virtual environments for them. This is one of the most important tools that most of the Python developers use.

### Why do we need a virtual environment?

Imagine a scenario where you are working on two web based python projects and one of them uses a Django 1.9 and the other uses Django 1.10 and so on. In such situations virtual environment can be really useful to maintain dependencies of both the projects.( Don't worry about Django now. It is a python framework used in the field of Web Development )

### When and where to use a virtual environment?

By default, every project on your system will use these same directories to store and retrieve site packages (third party libraries). How does this matter? Now, in the above example of two projects, you have two versions of Django. This is a real problem for Python since it can’t differentiate between versions in the “site-packages” directory. So both v1.9 and v1.10 would reside in the same directory with the same name. This is where virtual environments come into play. To solve this problem, we just need to create two separate virtual environments for both the projects.The great thing about this is that there are no limits to the number of environments you can have since they’re just directories containing a few scripts.

Virtual Environment should be used whenever you work on any Python based project. It is generally good to have one new virtual environment for every Python based project you work on. So the dependencies of every project are isolated from the system and each other.

Here is a short [tutorial](https://www.tutorialspoint.com.python-virtual-environment#:~:text=Creating%20Virtual%20Environments,the%20virtualenv%20tool%20with%20pip.) on virtual environments.

Also refer this [documentation](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/) for installing packages with pip when you are using virtual environments.

Refer [this](https://www.datacamp.com/community/tutorials/virtual-environment-in-python) tutorial if you are Anaconda user and want a better understanding of Virtual environments.

[This](https://www.youtube.com/watch?v=N5vscPTWKOk) video explains virtual environments and its implementation in a very good way. You should have a look at it.


# Learning with Hands-on code

Here is a problem for you to practise:

* Rock Paper Scissor - Make the game Rock Paper Scissor using python. Set up virtual environment in the directory that you use and install random library using pip. You can take help from this solution in case you are not able to solve it yourself. [Solution](https://thehelloworldprogram.com/python/python-game-rock-paper-scissors/)

       Input - "Rock"/ "Paper"/ "Scissor" (any 1)
       
       Raise an Error/Exception if the string entered does not match any of the above three.

       Output - First line contains computer's choice from Rock, Paper and Scissor based on random selection. Second line contains "You Win" / "Tie" / "You Lose" based on the conditions of the game.

       Conditions - Rock > Scissor, Scissor > Paper, Paper > Rock (> indicates L.H.S wins over R.H.S). In case of same choices, its a tie.

Now that you have covered most part of the course you can join online coding contests for improving your skills.

Here are some of the old contests which you can join and practise.

* [Hacker Rank Pythonist](https://www.hackerrank.com/contests/pythonist/challenges)
* [Hacker Rank Pythonist 2](https://www.hackerrank.com/contests/pythonist2/challenges)
* [Hacker Rank Pythonist 3](https://www.hackerrank.com/contests/pythonist3/challenges)


### Assignment - Week 4

Coming soon...

### Instructions to download the assignments:
1. Open on the respective `.ipynb` file on GitHub
2. In the upper right corner, there are several buttons and icons including the ones shown below. Click on the Raw Button.
       Raw | Blame
      --- | ---
      
3. The python notebook opens as raw text in browser. Right click->Save as OR just press CTRL + S. Save the notebook, open it using Jupyter Notebook you just installed and start learning! 


If you get stuck in any of the above questions, feel free to post them in the [Telegram](https://t.me/joinchat/OEr2Tk_ieMMmwihkBQVjFw) group. Additionally, you can also search for the problems online. Another aspect to becoming a good programmer is learning how to debug your code! it is very common to encounter error along the way of programming and in that case, try reading the error and understanding the reason behind it. More often than not, you may not be able to figure out yourself, the cause of the error. So, in that case, copy the error meassage and google it! You would be surprised how common such practices are and there are many forums where people may have already asked similar questions and have gotten solutions too! Stack Overflow is one such question and answer site for professional and enthusiast programmers. 

Congratualtions! You have successfully completed Week 4 of Python! Keep up the enthusiasm! 

Again, if you are having any difficulties with the course, please reach out to one of the moderators and we will surely help you out. 
<br>See you in Week 5!

<hr>













