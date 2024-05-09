/*****************************************************************************************************************
NAME:    AdventureWorks2019
PURPOSE: My AdventureWorks2019 script

MODIFICATION LOG:
Ver      Date        Author        Description
-----   ----------   -----------   -------------------------------------------------------------------------------
1.0     09/05/2024   DSambo       1. Built this script for EC IT143


RUNTIME: 
2s

NOTES: 
This is where I talk about what this script is, why I built it, and other stuff...
 
******************************************************************************************************************/

-- Q1:  Retrieve all columns from the BusinessEntity table?
-- A1: SELECT * FROM person.BusinessEntity

-- Q2: Retrieve the total sales amount from the PersonCreditCard table
-- A2: SELECT * FROM sales.personcreditcard

-- Q3: Identify the top three salespersons in terms of Bonus earned and how much sales did the make last year
-- A3: SELECT TOP 3 * FROM Sales.SalesPerson;
-- Q4: What is the most expensive product?
-- A4: SELECT TOP 5 * FROM production.product order by listprice;
-- Q5: Count the number of distinct products in the BusinessEntity table
-- A5: SELECT count(distinct productId) as NumberofProduct FROM production.product;
-- Q6:.
SELECT GETDATE(
	SELECT * FROM person.BusinessEntity
	SELECT * FROM sales.personcreditcard;
	SELECT TOP 3 * FROM Sales.SalesPerson;
	SELECT TOP 5 * FROM production.product order by listprice;
	SELECT count(distinct productId) as NumberofProduct FROM production.product;
	


) AS my_date;
