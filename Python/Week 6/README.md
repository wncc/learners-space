# Welcome to Week 6 of LS Python!
This week we will be covering the following topics:
* Python API
* Introduction to Web Scraping and Parsing 
  * Introduction to Selenium 

## Python APIs
Every website has an API or Application Programming Interface hosted on its web server, through which it distributes data avaliable on the web server. To use an API, you make a request to a remote web server, and retrieve the data you need. Retrieving data using APIs can be useful when the data on the web server is dynamic, that is, changing constantly, for example, stock price data. 
A good analogy for understanding APIs is that when you type in a URL, you request a webpage from the webserver, similarly, through an API you request data from the webserver. This data is returned in JSON format. 
* To get into more depth with Python APIs, checkout this link - **[Python API Tutorial](https://www.dataquest.io/blog/python-api-tutorial/)**


## Introduction to Web Scraping and Parsing
Web scraping is the process of accessing the HTML page of any website and then collecting data from that page. This is useful for many applications where you want data continously from websites in which data is dynamic, for instance, stock prices, or sports stats, or amazon product prices. Again, the idea is same as APIs, that is collect data from websites, but here instead of using the website's API for data, we use the HTML page of the website.
* Checkout this short video for an introduction to web scraping - **[Web Scraping Intro](https://www.youtube.com/watch?v=Ct8Gxo8StBU)**

Now lets go deeper into web scraping and build our own parser. For navigating through a webpage to extract only the useful information, we use a famous Python Library known as **BeautifulSoup**. You can checkout the documentation **[here](http://www.crummy.com/software/BeautifulSoup/)**. 
* Checkout this GfG tutorial on web scraping - **[Web Scraping GfG](https://www.geeksforgeeks.org/implementing-web-scraping-python-beautiful-soup/)**
* Go through this video series on web scraping - **[Video #1](https://www.youtube.com/watch?v=aIPqt-OdmS0)**, **[Video #2](https://www.youtube.com/watch?v=kRDrlvO-Oz0)**, **[Video #3](https://www.youtube.com/watch?v=sAuGH1Kto2I)**, **[Video #4](https://www.youtube.com/watch?v=FSH77vnOGqU)**. 

### Getting Started with Selenium 
Selenium is a framework which allows us to interact with the HTML elements of a website. So till now, we were only extracting data from a HTML webpage and then using it for different tasks. In addition to extracting data, Selenium allows us to interact with the webpage as well. So any interaction that you perform with a webpage can be automated using Selenium, for eg: Filling a form online, reading and extracting elements of the source code, etc. Now we will only be covering the basic of Selenium here, since Selenium in itself requires another course for learning. 
* Checkout this YouTube playlist on Introduction to Selenium - **[Selenium Tutorials Playlist](https://www.youtube.com/playlist?list=PLzMcBGfZo4-n40rB1XaJ0ak1bemvlqumQ)**. 

The videos in the playlist are made for absolute beginners, and walks through each and every step in detail, covering everything from installation (and troubleshooting) to introducing UnitTest frameworks. 
* Optionally, you can also checkout this link for reading tutorials - **[Selenium WebDriver Tutorials](https://www.guru99.com/selenium-tutorial.html)**. Keep in mind that this link also covers advanced tutorials on selenium webdrivers, so if you want to explore more of Selenium, you can go through them. 

## Assignment 6 - Automate Spotify with Python
For this week's assignment, you will be implementing a basic project in Python which takes a YouTube music video link, searches for the song title in Spotify and adds it to a playlist. 

What you need for the assignment - 
* **YouTube Data API** - This will be used for getting all the videos and playlists on YouTube. 
* **YouTube-dl Library** - This will be used for getting the artist and the song name from a youtube video. 
* **Spotify Web API** - This will be used for searching a song name on Spotify and then adding it to Liked Songs. 

