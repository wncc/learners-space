## About the data


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
