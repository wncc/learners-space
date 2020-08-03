# Welcome to Week 5 of Learner Space's Python! 

We are extremely glad that you have been constantly keeping up the enthusiasm and following the course. For the fifth week we will be covering the following topics:
* [File Handling](#file-handling)
* Use of major libraries - [Numpy](#use-of-numpy), [Pandas](#use-of-pandas), [Scipy](#use-of-scipy), [Matplotlib](#use-of-matplotlib)
* [GUI Development using Python](#gui-development-in-python)

This week and the subsequent one is aimed at introducing you to the diverse and wider applications of python. 
<hr>

## File Handling 

Files are named locations on disk to store related information. They are used to permanently store data in a non-volatile memory (e.g. hard disk). Since Random Access Memory (RAM) is volatile (which loses its data when the computer is turned off), we use files for future use of the data by permanently storing them. When we want to read from or write to a file, we need to open it first. When we are done, it needs to be closed so that the resources that are tied with the file are freed.

Hence, in Python, a file operation takes place in the following order:
1. Open a file
2. Read or write (perform operation)
3. Close the file

Head over to this [Notebook](./File_Handling/Week5-1.ipynb) to learn about Python functions for fucntions for file handling.

To read more about File Handling refer [this](https://www.geeksforgeeks.org/file-handling-python/)

<hr>

## Use of Numpy

##### What is NumPy?
NumPy is a python library used for working with arrays. It also has functions for working in domain of linear algebra, fourier transform, and matrices. NumPy stands for Numerical Python. It is an open source project and you can use it freely.

##### Why Use NumPy ?
In Python we have lists that serve the purpose of arrays, but they are slow to process. NumPy aims to provide an array object that is up to 50x faster that traditional Python lists. The array object in NumPy is called ndarray, it provides a lot of supporting functions that make working with ndarray very easy. Arrays are very frequently used in data science, where speed and resources are very important.

(Data Science: is a branch of computer science where we study how to store, use and analyze data for deriving information from it.)

##### Why is NumPy Faster Than Lists?
NumPy arrays are stored at one continuous place in memory unlike lists, so processes can access and manipulate them very efficiently. This behavior is called locality of reference in computer science. This is the main reason why NumPy is faster than lists. Also it is optimized to work with latest CPU architectures.

Head on to this [link](https://www.edureka.co/blog/python-numpy-tutorial/) for a brief explanation of numpy methods. Another reference for those aready a bit familiar and looking for a quick recap is [here](https://towardsdatascience.com/a-quick-introduction-to-the-numpy-library-6f61b7dee4db).

<hr>

## Use of Pandas

Pandas is an open-source library that is made mainly for working with relational or labeled data both easily and intuitively. It provides various data structures and operations for manipulating numerical data and time series. This library is built on the top of the NumPy library. Pandas is fast and it has high-performance & productivity for users.

##### Advantages of using Python
* Fast and efficient for manipulating and analyzing data.
* Data from different file objects can be loaded.
* Easy handling of missing data (represented as NaN) in floating point as well as non-floating point data
* Size mutability: columns can be inserted and deleted from DataFrame and higher dimensional objects
* Data set merging and joining.
* Flexible reshaping and pivoting of data sets
* Provides time-series functionality.
* Powerful group by functionality for performing split-apply-combine operations on data sets.

Head on to this [link](https://www.edureka.co/blog/python-pandas-tutorial/) for an overview of the library. If you are looking for quick recap just look at the video included in the previous link. Another reference for a more comprehensive overview is provided [here](https://pandas.pydata.org/pandas-docs/stable/getting_started/10min.html).

<hr>

## Use of SciPy

SciPy is a collection of mathematical algorithms and convenience functions built on the NumPy extension of Python. It adds significant power to the interactive Python session by providing the user with high-level commands and classes for manipulating and visualizing data. With SciPy, an interactive Python session becomes a data-processing and system-prototyping environment rivaling systems, such as MATLAB, IDL, Octave, R-Lab, and SciLab.

The additional benefit of basing SciPy on Python is that this also makes a powerful programming language available for use in developing sophisticated programs and specialized applications. Scientific applications using SciPy benefit from the development of additional modules in numerous niches of the software landscape by developers across the world. Everything from parallel programming to web and data-base subroutines and classes have been made available to the Python programmer. All of this power is available in addition to the mathematical libraries in SciPy.

Head on to this [link](https://www.edureka.co/blog/scipy-tutorial/) for an introduction to SciPy. Another reference for a more comprehensive overview is provided [here](https://www.tutorialspoint.com/scipy/scipy_quick_guide.htm). It includes the implementations of the varied subpackages.

<hr>

## Use of Matplotlib

Matplotlib is one of the most popular Python packages used for data visualization. It is a cross-platform library for making 2D plots from data in arrays. Matplotlib is written in Python and makes use of NumPy, the numerical mathematics extension of Python. It provides an object-oriented API that helps in embedding plots in applications using Python GUI toolkits such as PyQt, WxPythonotTkinter. It can be used in Python and IPython shells, Jupyter notebook and web application servers also.

Matplotlib has a procedural interface named the Pylab, which is designed to resemble MATLAB, a proprietary programming language developed by MathWorks. Matplotlib along with NumPy can be considered as the open source equivalent of MATLAB.

Head on to this [link](https://heartbeat.fritz.ai/introduction-to-matplotlib-data-visualization-in-python-d9143287ae39) for an introduction to data visualisation with matplotlib in python. Another reference for a more quick recap is provided [here](https://towardsdatascience.com/introduction-to-matplotlib-in-python-5f5a9919991f).

<hr>


# GUI development in Python

Python offers multiple options for developing GUI (Graphical User Interface). Most important are listed below-

* **Tkinter** − Tkinter is the Python interface to the Tk GUI toolkit shipped with Python. We would look this option in detail.

* **wxPython** − This is an open-source Python interface for wxWindows. Learn more [here](http://wxpython.org).

* **JPython** − JPython is a Python port for Java which gives Python scripts seamless access to Java class libraries on the local machin. Learn more [here](http://www.jython.org).

Out of all the GUI methods, tkinter is the most commonly used method. It is a standard Python interface to the Tk GUI toolkit shipped with Python. Python with tkinter is the fastest and easiest way to create the GUI applications. Tkinter provides a powerful object-oriented interface.

Creating a GUI application using Tkinter is an easy task. All you need to do is perform the following steps −
1. Import the Tkinter module.

2. Create the GUI application main window.

3. Add one or more of the above-mentioned widgets to the GUI application.

4. Enter the main event loop to take action against each event triggered by the user.

Head over to this [tutorial](https://www.geeksforgeeks.org/python-tkinter-tutorial/) to learn more about tkinter. You can also refer 
[this](https://www.javatpoint.com/python-tkinter) for a comprehensive overview of all UI widgets. 

For those prefering video tutorials [here](https://www.youtube.com/watch?v=VMP1oQOxfM0) is a good source to refer to. It is recommended to follow the video along with hands-on 
code writing and testing.

<hr>

## Assignment Week 5 
You can find this week's assignment [here](./Assignment5.md)

If you get stuck in any of the above questions, feel free to post them in the [Telegram](https://t.me/joinchat/OEr2Tk_ieMMmwihkBQVjFw) group. Additionally, you can also search for the problems online. Another aspect to becoming a good programmer is learning how to debug your code! It is very common to encounter error along the way of programming and in that case, try reading the error and understanding the reason behind it. More often than not, you may not be able to figure out the cause of the error yourself. So, in that case, copy the error message and google it! You would be surprised how common such practices are and there are many forums where people may have already asked similar questions and have got solutions too! Stack Overflow is one such question and answer site for professional and enthusiast programmers. 

Congratualtions! You have successfully completed Week 5 of Python! Keep up the enthusiasm! 

<br>See you in Week 6!

