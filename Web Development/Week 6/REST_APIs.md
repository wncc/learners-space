# Web Dev (LS 2020) Week 6: APIs in Django REST Framework

Django REST framework is a framework for django that easily allows you to create application programming interfaces for your applications. Let us first understand what an API is and what it does.

## Introduction to APIs

Whenever we create feature rich applications we also want to provide a method by which other users can use our application through their own code. This is useful because it allows people to extend our application's use beyond it's generic use case. For instance Google provides ways by which code can interact with gmail and calendar. Using this we can make a script/program that fetches the birthdays of our friends from calendar and then mail them using gmail automatically. Similarly if we created a blog application we would find it useful to be able to update or create new posts by code which would allow people to automate or use other services to interact with your application. This interaction is provided by using Application Programming Interfaces (APIs).

Generally we would however be using a special class of APIs called as RESTful APIs. REST stands for Representational State Transfer. It is a set of rules that developers follow when they create their API. One of these rules states that you should be able to get a piece of data (called a resource) when you link to a specific URL. Basically your application will have certain URLs and you can send data to these URLs similar to how forms are submitted. Once you have authenticated your user over this URL you will take the data and make a change in the underlying database of your application. Similarly you have some URLs from which you can get data. For instance if you have a blog application then using a url like http://myblog.com/api/get_posts/ would provide all the posts of your blog in a data format.

Generally a data format called JSON is used to transmit data over APIs. You can read about it [here](https://www.w3schools.com/js/js_json_intro.asp). Refer to this [link](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Introduction) by Mozilla and this [resource](https://www.geeksforgeeks.org/introduction-to-apis/) on GeeksForGeeks for more information on APIs.

## Django REST Framework

In general creating REST APIs is not very simple as one has to take care of endpoints and ensure that no leak of state is there. One would have to manually configure every url and point it to a view which would get the data from a model. Instead of doing this by ourselves, we should use plugins that have already abstracted this for us. For Django there is a very useful framework called Django REST Framework that does this for us. Similarly other modules like Flask have their own plugins like Flask-Restful.

Django REST framework makes serialisation very easy. Writing little code you can directly output your models via a json format through the api url. For instance you can make an API URL for your posts through the posts model that you had defined in Django. Refer to this [basic tutorial](https://medium.com/swlh/build-your-first-rest-api-with-django-rest-framework-e394e39a482c) to create a simple API using Django REST. Django REST takes care of the hard stuff for you and directly interacts with the model exposing it through api endpoints.

Refer to this [tutorial](https://djangostars.com/blog/rest-apis-django-development/) by DjangoStars for more information. This also shows how you can set up POST endpoints for sending information to your application via http requests.

This [link](https://www.django-rest-framework.org/tutorial/quickstart/) will take you to the official tutorial that will guide you through the advanced features of this framework. Please do make sure to go through the API guide also given in the previous link.