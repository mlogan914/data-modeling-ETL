# Mini Project -- Data Warehouse Modeling using Snowflake via DBeaver

## 1. Project Description
- Step 1: Create a data model for a data warehouse (Snowflake).
- Step 2: Write the ETL script (DDL, DML) to transform the data from the original tables to the data model.

## 2. About the Data
The Sakila database (originally created by MySQL) is a normalised schema modelling a DVD rental store, featuring films, actors, film-actor relationships, and a central inventory table that connects films, stores, and rentals. 

The database relationship in the original database looks like this:
![sakila_os_diagram](https://user-images.githubusercontent.com/74939090/197332630-f9508613-de3e-4698-90a3-f7d1902d70c6.png)



## 3. Business Requirements
In this project, we need to make a data model to meet the following requirements from the managemental team:

1. List the total revenue of each store everyday.
2. List the total revenue of totally everyday.
3. List the top store according to their weekly revenue every week.
4. List top sales clerk who have the most sales each day/week/month.
5. Which film is the top film each week/month in each store/totally?
6. Who are our top 10 customers each month/year?
7. Is there any store the sales is in a decline trend (within the recent 4 weeks the avg sales of each week is declining).

The goal is to create a data model where the user can easily query using simple SQL queries SELECT, GROUP BY, JOIN.

## 4. Project Steps
1. Load the origial data into the landing area.
2. Analyze the Business Requirements and translate the requirements into the technical requirements (rough formulas).
3. Consider the Grain of the data model based the above Requirements; Consider the atomic row of a fact table.
4. Decide what dimension tables will be used in the data model. Also consider what columns to include into the dimensions.
5. Define the fact table.
6. Create the dimension and fact tables in the Snowflake data warehouse; Make sure the data model is in a different schema.
7. Write ETL script to transform data from the original tables to the target tables in the data model.
