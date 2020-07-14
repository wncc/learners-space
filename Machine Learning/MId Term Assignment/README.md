# Mid-Term Assignment
In this assignment, you will put into practice some of the key principles and techniques you have learned in the course upto now. You are free to use any algorithm out of all of those which you have learned in this course,to implement regression models to the datasets. **To complete this assignment you have to complete both the problems, to get a detailed description about them, refer below**.<br/> <br/>

## Problem 1:

We find this as a very good dataset for you to practice your hands on exploring data and building regression models.

### Problem Overview
In 1998, the Adventure Works Cycles company collected a large volume of data about their existing customers, including demographic features and information about purchases they have made. The company is particularly interested in analyzing customer data to determine any apparent relationships between demographic features known about the customers and the likelihood of a customer purchasing a bike. Additionally, the analysis should endeavor to determine whether a customer's average monthly spend with the company can be predicted from known customer characteristics.

To complete this problem, you must tackle two challenges:
- Challenge 1: Explore the data and gain some insights into Adventure Works customer characteristics and purchasing behavior.
- Challenge 2: Build a regression model to predict customer purchasing behavior.


### About the Data
To know about the data, refer to [this](https://github.com/wncc/learners-space/blob/master/Machine%20Learning/MId%20Term%20Assignment/About%20the%20data.md) link.

### Challenge 1: Data Exploration

To complete this challenge:
1. Download the Adventure Works data files present inside this folder.
2. Clean the data by replacing any missing values and removing duplicate rows. In this dataset, each customer is identified by a unique customer ID. The most recent version of a duplicated record should be retained.
3. Explore the data by calculating summary and descriptive statistics for the features in the dataset, calculating correlations between features, and creating data visualizations to determine apparent relationships in the data.
4. Based on your analysis of the customer data after removing all duplicate customer records, answer the questions in this [form](https://forms.gle/CJ7cLSZY145yBnmh9).

### Challenge 2: Regression 
Create a regression model that predicts the average monthly spend of a new customers.

To complete this challenge:
1. Use the Adventure Works Cycles customer data you worked with in challenge 1 to create a regression model that predicts a customer's average monthly spend. The model should predict average monthly spend for new customers for whom no information about average monthly spend or previous bike purchases is available.
2. Download the test data. This data includes customer features but does not include bike purchasing or average monthly spend values.
3. Use your model to predict on the corresponding test dataset. Don't forget to apply what you've learned throughout this course upto now.
4. For every Customer in the dataset, submission files should contain two columns: CustomerID and Prediction1.
The file should contain a header and have the format given below to:

> CustomerID,Prediction1 <br/>
> 18988,1 <br/>
> 29135,0 <br/>
> 12156,1 <br/>
> 13749,1 <br/>
> etc. <br/>

For the submission, you will have to provide a github repo link/drive link/google colab notebook to a form we will be releasing soon.
## Problem 2:
You are given a dataset of points in `data.json` of the form [x, y, label]. The label is either 0 or 1. You need to implement logistic regression to predict the label of a dataset similar to `data.json`. Please note that the test data is not given, this is the training data. However both the training data and the test data will follow the same distribution (so the curve you see will indeed be the decision boundary). Create a python file that takes in `data.json` as input in the same directory (if this is not followed then you will be penalised).

(Hint: The data can be fit by a four degree polynomial of the form x^4 + x^3y + x^2y^2 along with lower degree terms..)

***We have made these assignments for you to have a better learning experience, if you get stuck discuss to a moderator about it and refrain from plagiarism. All the best, it's time to get started.***

### Last Date of Submission: July 19, Sunday



