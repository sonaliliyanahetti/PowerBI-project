STEP 1: Import data set from difference sources.
Load excel and csv files  normal way. Then import sales csv three files according to different three years as one folder after transform data.

STEP 2: Data preparation
>use first row as the headers in some tables.
>merge first and last name to one column and rename it as full name.
>Create username by using "@" in the email address as the delimiter.
>Check data types of the columns and change to relevant data type.
>Check the quality of the columns
>Convert numerical data to categorical(Create new conditional column using AnnualIncome)
>Rounding floating values to two decimal places in product Query
>Create a custom column as Discount price by imaging 25% of discount and round off values to two decimal places.		
>Add new columns to calendar query (correct date format is dd/mm/y)
>Transpose the Manufacture query and then enable load data because Manufacturing query has no connection with other queries.


STEP 3:Data Modeling
Relationships created
>Products and Returns tables using the Productkey
>Products and Product_Subcategories tables using the ProductSubcategorykey 
>Product_Subcategories and Product_Categories tables using the ProductCategorykey
>Sales and Customers tables using the Customerkey column
>Sales and Territories using TerritoryKey
>OrderDate column in the Sales table to the Date column in the Calendar table


STEP 4:Power BI Desktop – Data Exploration
>Add a Data Analysis Expressions (DAX) as Unit price in sales query.(The RELATED DAX function is used to return a related value from another table)
>create a measure an type a DAX formular to Total orders using DISTINCTCOUNT()

![Screenshot 2024-12-19 160254](https://github.com/user-attachments/assets/893bd000-914f-415e-86b0-aa3fd787c926)
