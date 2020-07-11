# Mid-Term Assignment
In this assignment, you will put into practice some of the key principles and techniques you have learned in the course upto now. You are free to use any algorithm out of all of those which you have learned in this course,to implement regression models to the datasets. To complete this assignment you have to complete both the problems, to get a detailed description about them, refer below.<br/> <br/>

## Problem 1:

We find this as a very good dataset for you to practice your hands on exploring data and building regression models.

### Problem Overview
In 1998, the Adventure Works Cycles company collected a large volume of data about their existing customers, including demographic features and information about purchases they have made. The company is particularly interested in analyzing customer data to determine any apparent relationships between demographic features known about the customers and the likelihood of a customer purchasing a bike. Additionally, the analysis should endeavor to determine whether a customer's average monthly spend with the company can be predicted from known customer characteristics.

In complete this problem, you must tackle three challenges:
- Challenge 1: Explore the data and gain some insights into Adventure Works customer characteristics and purchasing behavior.
- Challenge 2: Build a regression model to predict customer purchasing behavior.


### About the Data
This data consists of three files, containing data that was collected on January 1st 1998.
Clone this repo and use the folders provided in this repo <br/>

AdvWorksCusts.csv 


Customer demographic data consisting of the following fields:

    CustomerID (integer): A unique customer identifier.
    Title (string): The customer's formal title (Mr, Mrs, Ms, Miss Dr, etc.)
    FirstName (string): The customer's first name.
    MiddleName (string): The customer's middle name.
    LastName (string): The customer's last name.
    Suffix (string): A suffix for the customer name (Jr, Sr, etc.)
    AddressLine1 (string): The first line of the customer's home address.
    AddressLine2 (string): The second line of the customer's home address.
    City (string): The city where the customer lives.
    StateProvince (string): The state or province where the customer lives.
    CountryRegion (string): The country or region where the customer lives.
    PostalCode (string): The postal code for the customer's address.
    PhoneNumber (string): The customer's telephone number.
    BirthDate (date): The customer's date of birth in the format YYYY-MM-DD.
    Education (string): The maximum level of education achieved by the customer:
        Partial High School
        High School
        Partial College
        Bachelors
        Graduate Degree
    Occupation (string): The type of job in which the customer is employed:
        Manual
        Skilled Manual
        Clerical
        Management
        Professional
    Gender (string): The customer's gender (for example, M for male, F for female, etc.)
    MaritalStatus (string): Whether the customer is married (M) or single (S).
    HomeOwnerFlag (integer): A Boolean flag indicating whether the customer owns their own home (1) or not (0).
    NumberCarsOwned (integer): The number of cars owned by the customer.
    NumberChildrenAtHome (integer): The number of children the customer has who live at home.
    TotalChildren (integer): The total number of children the customer has.
    YearlyIncome (decimal): The annual income of the customer.

AW_AveMonthSpend.csv

Sales data for existing customers, consisting of the following fields:

    CustomerID (integer): The unique identifier for the customer.
    AveMonthSpend (decimal): The amount of money the customer spends with Adventure Works Cycles on average each month.

AW_BikeBuyer.csv

Sales data for existing customers, consisting of the following fields:

    CustomerID (integer): The unique identifier for the customer.
    BikeBuyer (integer): A Boolean flag indicating whether a customer has previously purchased a bike (1) or not (0).

### Challenge 1: Data Exploration

To complete this challenge:
1. Download the Adventure Works data files.
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
The file should contain a header and have the format given below to [this]((** koi naya gmail count bna le submissions k liye? **) gmail id

> CustomerID,Prediction1 <br/>
> 18988,1 <br/>
> 29135,0 <br/>
> 12156,1 <br/>
> 13749,1 <br/>
> etc. <br/>

## Problem 2:

** Pradipta will add here by 3 tonight **




