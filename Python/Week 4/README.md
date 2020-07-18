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

### Dice Roll

* Start a Virtual Environment in a directory and install packages like random, math, numpy, matplotlib, scipy using pip. 

* Run a Simulation of rolling 3 dice 1000 times and plot Probability Distribution Curve for Sum of the numbers on 3 dice. 

* The points connecting the curve shall only contain integers for their X-coordinate. X-axis should contain "Sum of the numbers on 3 dice" and "Y-axis should contain probability of Sum of numbers to be X". 

* Apply "Savitzy-Golay filter"( or any other curve smoothening tool ) on the curve and plot another "smooth" version of 1st curve on the same graph using a different color. Note that this filter would plot a polynomial curve and may not pass through the exact points. This is just to get an approximate shape of the curve. You may take help from [here](https://stackoverflow.com/questions/20618804/how-to-smooth-a-curve-in-the-right-way)

* Plot a Bar-graph of probabilities of Sum of numbers on 3 dice on a different plot.

* Make sure you set proper scale for the axes and label the axes. Also give title to the 2 plots.

* You are only allowed to use packages mentioned in the 1st point.

* Submission - Submit the file Your_Name(1).py ('Your_Name' is to be replaced by your name) along with 2 plots in a Google drive folder or Github repository.

Refrain from using Notebooks for this assignment. For basic plotting skills with matplotlib you can refer [this](https://www.wncc-iitb.org/wiki/index.php/Data_Analytics) article on WnCC's Grundy (wiki). Purpose of this assignment is to see how you can handle new libraries of python by referring to their documentations online and to give you a brief introduction to the field of Data Visualization.

### Virus Spread Simulation (Basic)

* Create a two-dimensional matrix of dimention 100 * 150 containing 15,000 entries with value 0. Set the entry (50,75) to be 1.

* 8 random entries swap with another set of 8 random entries.

* ![Visual representation](https://www.researchgate.net/profile/Igor_Florinsky/publication/220650043/figure/fig5/AS:669074258395143@1536531142223/The-565-window-1-25-are-numbers-of-the-window-nodes-w-is-grid-size-metres.png)

* If 13 is the selected entry, 7,8,9,12,14,17,18,19 are 1st neighbours and 1,2,3,4,5,6,10,11,15,16,20,21,22,23,24,25 are 2nd neighbours.

* 1st neighbours of an entry containing 1 each have a 0.25 probability of getting converted to 1.

* 2nd neighbours of an entry containing 1 each have a 0.08 probability of getting converted to 1.

* Each entry has an independent probability of getting converted to 1 depending upon its relative position to an entry containing 1.

* Note that it is not mandatory for one of the neighbours to be converted into 1.

* Keep repeating the process till every entry becomes 1.

* Plot 1: Number of ones in the matrix vs Number of iterations

* Plot 2: Change in number of ones in each iteration vs Number of iterations

* Print the peak value in Plot 2. Make sure you label the axes in both the plots.

* Submission: Submit the file Your_Name(2).py ('Your_Name' is to be replaced by your name) along with plot 1 and plot 2 in a Google drive folder or Github repository

You are free to use anything you want in this problem. Stack Overflow, Github, Geeks for Geeks are some of the widely used platforms by coders to discuss various things like certain methods to solve a problem, resolving errors, etc. Finally as the name suggests, this is a very basic Virus spread simulation in a rectangular large area with 0s turning into 1 depiicting a person getting infected with virus. Random shuffling means travelling. You can always try modifying this problem by adding a recovery rate, consider time taken to detect virus after person has been infected and various things but this is not expected as far as this assignment is concerned.

<hr>

If you get stuck in any of the above questions, feel free to post them in the [Telegram](https://t.me/joinchat/OEr2Tk_ieMMmwihkBQVjFw) group. Additionally, you can also search for the problems online. Another aspect to becoming a good programmer is learning how to debug your code! it is very common to encounter error along the way of programming and in that case, try reading the error and understanding the reason behind it. More often than not, you may not be able to figure out yourself, the cause of the error. So, in that case, copy the error meassage and google it! You would be surprised how common such practices are and there are many forums where people may have already asked similar questions and have gotten solutions too! Stack Overflow is one such question and answer site for professional and enthusiast programmers. 

Congratualtions! You have successfully completed Week 4 of Python! Keep up the enthusiasm! 

Again, if you are having any difficulties with the course, please reach out to one of the moderators and we will surely help you out. 
<br>See you in Week 5!

<hr>













