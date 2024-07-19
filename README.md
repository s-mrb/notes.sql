- [Basic](#basic)
  - [Distinct](#distinct)
  - [AND, OR, NOT](#and-or-not)
  - [ORDER BY](#order-by)
  - [INSERT INTO](#insert-into)
  - [NULL](#null)
  - [UPDATE](#update)
  - [DELETE](#delete)
  - [TOP](#top)
  - [LIMIT](#limit)
  - [FETCH FIRST](#fetch-first)
  - [MIN/MAX](#minmax)
  - [COUNT](#count)
  - [AVG/SUM](#avgsum)
  - [LIKE](#like)
  - [WILDCARDS](#wildcards)
  - [IN](#in)
  - [BETWEEN](#between)
  - [NOT BETWEEN](#not-between)
  - [ALIAS](#alias)
  - [JOIN](#join)
  - [SELF JOIN](#self-join)
  - [UNION](#union)
  - [GROUP BY](#group-by)
  - [HAVING](#having)
  - [EXISTS](#exists)
  - [ANY/ALL](#anyall)
  - [SELECT INTO](#select-into)
  - [INSERT INTO](#insert-into-1)
  - [CASE](#case)
  - [IFNULL/ISNULL/COALESCE](#ifnullisnullcoalesce)
  - [STORED PROCEDURE](#stored-procedure)
  - [COMMENTS](#comments)
  - [DATABASE](#database)
  - [Table](#table)
    - [CREATE](#create)
    - [ALTER](#alter)
    - [TRUNCATE](#truncate)
  - [CONSTRAINTS](#constraints)
  - [NOT NULL](#not-null)
  - [UNIQUE](#unique)
  - [PRIMARY KEY](#primary-key)
  - [FOREIGN KEY](#foreign-key)
  - [CHECK](#check)
  - [DEFAULT](#default)
  - [INDEX](#index)
  - [AUTO INCREMENT](#auto-increment)
  - [VIEW](#view)
  - [3 types of Commands](#3-types-of-commands)
  - [DDL](#ddl)
  - [Date and Time](#date-and-time)
  - [To add date](#to-add-date)
  - [CREATE DOMAIN](#create-domain)
  - [SQL Referential Integrity \& Updates](#sql-referential-integrity--updates)
  - [ALTER](#alter-1)
  - [INDEX](#index-1)
  - [Trigger](#trigger)
  - [TRANSACTION](#transaction)
  - [TRANSACTION SYNTAX](#transaction-syntax)
  - [SAVEPOINT and ROLLBACK](#savepoint-and-rollback)
  - [UPDATE](#update-1)
  - [PRIVILEGES](#privileges)
  - [ROUND](#round)
  - [LENGTH](#length)
  - [LEFT](#left)
  - [Correlated Subquery](#correlated-subquery)
  - [Position of Having](#position-of-having)
  - [Drop](#drop)
  - [Use NULL](#use-null)
  - [offset](#offset)
  - [CTE](#cte)
  - [Why Columnar Databases are faster for retrieval](#why-columnar-databases-are-faster-for-retrieval)
  - [Sharding](#sharding)
  - [Index](#index-2)
  - [View](#view-1)
  - [Is View just a stored query or the is it the stored data from query?](#is-view-just-a-stored-query-or-the-is-it-the-stored-data-from-query)
  - [If view is not stored data and just a query then how can it speed up the data retrieval?](#if-view-is-not-stored-data-and-just-a-query-then-how-can-it-speed-up-the-data-retrieval)
  - [Columnar Databases](#columnar-databases)
  - [Normalization](#normalization)
  - [2NF](#2nf)
  - [Partial dependency](#partial-dependency)
  - [3NF](#3nf)
  - [Transitive dependency](#transitive-dependency)
  - [4NF](#4nf)
  - [Non-trivial Multi-valued dependency](#non-trivial-multi-valued-dependency)
  - [Types of indexes](#types-of-indexes)
  - [WINDOW FUNCTIONS](#window-functions)
  - [Modules in DBMS](#modules-in-dbms)
  - [Two Tier Architecture](#two-tier-architecture)
  - [Three Tier](#three-tier)
  - [Data Abstraction in Three Schema Architecture](#data-abstraction-in-three-schema-architecture)
  - [Data Abstraction Leads to Data Independence](#data-abstraction-leads-to-data-independence)
  - [Schema](#schema)
  - [Data Models](#data-models)
  - [Relational Data Model](#relational-data-model)
  - [Relational Constraints](#relational-constraints)
- [MUST SEE](#must-see)
  - [How to subtract 30 days from the current date using SQL Server](#how-to-subtract-30-days-from-the-current-date-using-sql-server)
  - [managers with at least five direct reports.](#managers-with-at-least-five-direct-reports)
  - [The Number of Employees Which Report to Each Employee](#the-number-of-employees-which-report-to-each-employee)
  - [Compare consecutive rows of table](#compare-consecutive-rows-of-table)
  - [Add a new column and its conditional  value](#add-a-new-column-and-its-conditional--value)
  - [Add a column with Running aggregate](#add-a-column-with-running-aggregate)
  - [FETCH AND OFFSET](#fetch-and-offset)
    - [Conditional rendering of values of a column](#conditional-rendering-of-values-of-a-column)
  - [Delete Duplicate Emails](#delete-duplicate-emails)
  - [Summary creation of category](#summary-creation-of-category)
  - [Write a solution to report the movies with an odd-numbered ID and a description that is not "boring".](#write-a-solution-to-report-the-movies-with-an-odd-numbered-id-and-a-description-that-is-not-boring)
  - [Write a solution to find all dates' Id with higher temperatures compared to its previous dates (yesterday).](#write-a-solution-to-find-all-dates-id-with-higher-temperatures-compared-to-its-previous-dates-yesterday)
  - [](#)
  - [NOTE](#note)
  - [Note](#note-1)
  - [Order By with CASE](#order-by-with-case)
  - [VV IMP](#vv-imp)
  - [VV IMP: CASE IN SELECT](#vv-imp-case-in-select)
  - [query quality](#query-quality)
- [Example](#example)
  - [XOR](#xor)
  - [Order By Multiple Cols](#order-by-multiple-cols)
  - [Bypass Null](#bypass-null)
  - [List each continent and the name of the country that comes first alphabetically.](#list-each-continent-and-the-name-of-the-country-that-comes-first-alphabetically)
  - [Group By and Having](#group-by-and-having)
  - [See](#see)
- [Misc](#misc)
  - [HAVING vs WHERE](#having-vs-where)
  - [How to make stored Procedures](#how-to-make-stored-procedures)
  - [What are the differences between PRIMARY, UNIQUE, INDEX and FULLTEXT when creating MySQL tables?](#what-are-the-differences-between-primary-unique-index-and-fulltext-when-creating-mysql-tables)
    - [Differences](#differences)
    - [Similarities](#similarities)
- [functions](#functions)
  - [SUBSTRING](#substring)
  - [LEAD and LAG](#lead-and-lag)
- [WINDOW FUNCTIONS](#window-functions-1)
  - [Link](#link)
  - [Dataset](#dataset)
    - [Rank Rentals by Price](#rank-rentals-by-price)
    - [Find 2nd Giftcard-Purchasing Customer](#find-2nd-giftcard-purchasing-customer)
    - [Calculate Running Total for Payments](#calculate-running-total-for-payments)
  - [Dataset](#dataset-1)
    - [Calculate Moving Average for Scores](#calculate-moving-average-for-scores)
    - [Find the Difference Between Procedure Prices](#find-the-difference-between-procedure-prices)
    - [Find the Difference Between the Current and Best Prices](#find-the-difference-between-the-current-and-best-prices)
    - [Find the Best Doctor per Procedure](#find-the-best-doctor-per-procedure)
- [Links](#links)


# Basic
## Distinct

The SELECT DISTINCT statement is used to return only distinct (different) values.

Inside a table, a column often contains many duplicate values; and sometimes you only want to list the different (distinct) values.

```sql
¶¶
SELECT DISTINCT Country FROM Customers;

¶¶
SELECT Count(*) AS DistinctCountries
FROM (SELECT DISTINCT Country FROM Customers);
```

## AND, OR, NOT

```sql
SELECT * FROM Customers
WHERE Country='Germany' AND City='Berlin';


SELECT * FROM Customers
WHERE City='Berlin' OR City='München';


SELECT * FROM Customers
WHERE NOT Country='Germany';
```

## ORDER BY

- sorts the records in ascending order by default.

```sql
¶¶
SELECT * FROM Customers
ORDER BY Country DESC;

```

- ORDER BY Several Columns

> orders by Country, but if some rows have the same Country, it orders them by CustomerName:

```sql
¶¶
SELECT * FROM Customers
ORDER BY Country, CustomerName;

```
## INSERT INTO

```sql
--  specify columns 
INSERT INTO table_name (column1, column2, column3, ...)
VALUES (value1, value2, value3, ...);

-- all cols
INSERT INTO table_name
VALUES (value1, value2, value3, ...);
```

## NULL

A field with a NULL value is a field with no value.

If a field in a table is optional, it is possible to insert a new record or update a record without adding a value to this field. Then, the field will be saved with a NULL value.

**TEST NULL**
It is not possible to test for NULL values with comparison operators, such as =, <, or <>.

```sql
¶¶
SELECT column_names
FROM table_name
WHERE column_name IS NULL;

¶¶
SELECT column_names
FROM table_name
WHERE column_name IS NOT NULL;
```

## UPDATE

```sql
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

## DELETE

```sql
DELETE FROM Customers WHERE CustomerName='Alfreds Futterkiste';

```
> If you omit the WHERE clause, all records in the table will be deleted!

## TOP

```sql

¶¶
SELECT TOP 3 * FROM Customers;

SELECT TOP 50 PERCENT * FROM Customers;
```

## LIMIT

```sql
SELECT * FROM Customers
LIMIT 3;
```

## FETCH FIRST

```sql
SELECT * FROM Customers
FETCH FIRST 50 PERCENT ROWS ONLY;

SELECT * FROM Customers
FETCH FIRST 5 ROWS ONLY;
```

## MIN/MAX

```sql
SELECT MIN(column_name)
FROM table_name
WHERE condition;
```

## COUNT

```sql
SELECT COUNT(column_name)
FROM table_name
WHERE condition;
```

## AVG/SUM

```sql
SELECT AVG(column_name)
FROM table_name
WHERE condition;
```


## LIKE

There are two wildcards often used in conjunction with the LIKE operator:

- The percent sign (%) represents zero, one, or multiple characters
- The underscore sign (_) represents one, single character

```sql
SELECT column1, column2, ...
FROM table_name
WHERE columnN LIKE pattern;
```

The following SQL statement selects all customers with a CustomerName that does NOT start with "a":

```sql
SELECT * FROM Customers
WHERE CustomerName NOT LIKE 'a%';
```

## WILDCARDS

[ ] -> 
- Represents any single character within the brackets	
- h[oa]t finds hot and hat, but not hit

^ -> 
- Represents any character not in the brackets	
- h[^oa]t finds hit, but not hot and hat

- ->
- Represents any single character within the specified range
- c[a-b]t finds cat and cbt



°°°
The two following SQL statements select all customers with a City NOT starting with "b", "s", or "p":

```sql
SELECT * FROM Customers
WHERE City LIKE '[!bsp]%';
```

```sql
SELECT * FROM Customers
WHERE City NOT LIKE '[bsp]%';
```

## IN
The IN operator is a shorthand for multiple OR conditions.

```sql
SELECT column_name(s)
FROM table_name
WHERE column_name IN (value1, value2, ...);
```

## BETWEEN
The BETWEEN operator selects values within a given range. The values can be numbers, text, or dates.

The BETWEEN operator is inclusive: begin and end values are included. 

```sql
SELECT * FROM Products
WHERE Price BETWEEN 10 AND 20;

SELECT * FROM Orders
WHERE OrderDate BETWEEN '1996-07-01' AND '1996-07-31';
```

## NOT BETWEEN

To display the products outside the range of the previous example, use NOT BETWEEN

## ALIAS
```sql
SELECT o.OrderID, o.OrderDate, c.CustomerName
FROM Customers AS c, Orders AS o
WHERE c.CustomerName='Around the Horn' AND c.CustomerID=o.CustomerID;
```


## JOIN
A JOIN clause is used to combine rows from two or more tables, based on a related column between them.


- **(INNER) JOIN**: Returns records that have matching values in both tables
- **LEFT (OUTER) JOIN**: Returns all records from the left table, and the matched records from the right table
- **RIGHT (OUTER) JOIN**: Returns all records from the right table, and the matched records from the left table
- **FULL (OUTER) JOIN**: Returns all records when there is a match in either left or right table. 


**MATCHING VALUE?** 
Value of specified column of left table in the specified column of the right table. 

```sql
SELECT Orders.OrderID, Customers.CustomerName, Orders.OrderDate
FROM Orders
INNER JOIN Customers ON Orders.CustomerID=Customers.CustomerID;
```

## SELF JOIN

```sql
SELECT A.CustomerName AS CustomerName1, B.CustomerName AS CustomerName2, A.City
FROM Customers A, Customers B
WHERE A.CustomerID <> B.CustomerID
AND A.City = B.City
ORDER BY A.City;
```

## UNION
- Every SELECT statement within UNION must have the same number of columns
- The columns must also have similar data types
- The columns in every SELECT statement must also be in the same order

```sql
SELECT column_name(s) FROM table1
UNION
SELECT column_name(s) FROM table2;
```

°°°
The UNION operator selects only distinct values by default. To allow duplicate values, use UNION ALL

## GROUP BY

- groups rows that have the same values into summary rows, like "find the number of customers in each country"
- often used with aggregate functions

```sql
SELECT COUNT(CustomerID), Country
FROM Customers
GROUP BY Country;
```

## HAVING

- The HAVING clause was added to SQL because the WHERE keyword cannot be used with aggregate functions.

```sql
SELECT COUNT(CustomerID), Country
FROM Customers
GROUP BY Country
HAVING COUNT(CustomerID) > 5
ORDER BY COUNT(CustomerID) DESC;
```

## EXISTS 

- returns TRUE if the subquery returns one or more records. 


The following SQL statement returns TRUE and lists the suppliers with a product price less than 20:


```sql
SELECT SupplierName
FROM Suppliers
WHERE EXISTS (SELECT ProductName FROM Products WHERE Products.SupplierID = Suppliers.supplierID AND Price < 20);
```

## ANY/ALL 

°°° 
Select all the students whose age greater than at least one lecturer

```sql
SELECT * FROM student 
WHERE age > ANY 
( SELECT age FROM lecturer ) ;
```

°°° 
Select all the students whose age greater than all of the lecturers

```sql
SELECT * FROM student 
WHERE age > ALL
( SELECT age FROM lecturer ) ;
```

- [review](https://www.youtube.com/watch?v=nD7JAdEQYAE)


## SELECT INTO

°°°
Table backup in the same database

```sql
SELECT * INTO CustomersBackup2017
FROM Customers;
```

°°°
Table backup in another database

```sql
SELECT * INTO CustomersBackup2017 IN 'Backup.mdb'
FROM Customers;
```

°°°
Copy just the schema

```sql
SELECT * INTO newtable
FROM oldtable
WHERE 1 = 0;
```
> NOTE the difference

```sql
BACKUP DATABASE databasename
TO DISK = 'filepath';
```

## INSERT INTO

```sql
INSERT INTO Customers (CustomerName, City, Country)
SELECT SupplierName, City, Country FROM Suppliers;
```

## CASE

```sql
SELECT OrderID, Quantity,
CASE
    WHEN Quantity > 30 THEN 'The quantity is greater than 30'
    WHEN Quantity = 30 THEN 'The quantity is 30'
    ELSE 'The quantity is under 30'
END AS QuantityText
FROM OrderDetails;
```


```sql
SELECT CustomerName, City, Country
FROM Customers
ORDER BY
(CASE
    WHEN City IS NULL THEN Country
    ELSE City
END);
```

## IFNULL/ISNULL/COALESCE

```sql
SELECT ProductName, UnitPrice * (UnitsInStock + IFNULL(UnitsOnOrder, 0))
FROM Products;

SELECT ProductName, UnitPrice * (UnitsInStock + ISNULL(UnitsOnOrder, 0))
FROM Products;

SELECT ProductName, UnitPrice * (UnitsInStock + COALESCE(UnitsOnOrder, 0))
FROM Products;
```

## STORED PROCEDURE
```sql
CREATE PROCEDURE SelectAllCustomers @City nvarchar(30), @PostalCode nvarchar(10)
AS
SELECT * FROM Customers WHERE City = @City AND PostalCode = @PostalCode
GO;
```
°°° 
**EXECUTE**
```sql
EXEC SelectAllCustomers @City = 'London', @PostalCode = 'WA1 1DP';
```

## COMMENTS

- --
- /**/



## DATABASE
```sql
CREATE DATABASE databasename;

DROP DATABASE databasename;

BACKUP DATABASE databasename
TO DISK = 'filepath';

BACKUP DATABASE databasename
TO DISK = 'filepath'
WITH DIFFERENTIAL;
```
°°°
differential back up only backs up the parts of the database that have changed since the last full database backup.

## Table

### CREATE

```sql
CREATE TABLE Persons (
    PersonID int,
    LastName varchar(255),
    FirstName varchar(255),
    Address varchar(255),
    City varchar(255)
);

CREATE TABLE TestTable AS
SELECT customername, contactname
FROM customers;
```

### ALTER

```sql
ALTER TABLE Customers
ADD Email varchar(255);

ALTER TABLE Customers
DROP COLUMN Email;

ALTER TABLE table_name
ALTER COLUMN column_name datatype;

ALTER TABLE table_name
RENAME COLUMN old_name to new_name;
```

```sql
RENAME TABLE old_table_name TO new_table_name;
```

### TRUNCATE

```sql
TRUNCATE TABLE table_name;
```

## CONSTRAINTS

- NOT NULL
- UNIQUE
- PRIMARY KEY
- FOREIGN KEY
- CHECK
- DEFAULT
- CREATE INDEX

## NOT NULL
```sql

CREATE TABLE Persons (
    ID int NOT NULL,
    LastName varchar(255) NOT NULL,
    FirstName varchar(255) NOT NULL,
    Age int
);

ALTER TABLE Persons
ALTER COLUMN Age int NOT NULL;
```

## UNIQUE
```sql
CREATE TABLE Persons (
    ID int NOT NULL UNIQUE,
    LastName varchar(255) NOT NULL,
    FirstName varchar(255),
    Age int
);

ALTER TABLE Persons
ADD UNIQUE (ID);

ALTER TABLE Persons
ADD CONSTRAINT UC_Person UNIQUE (ID,LastName)
```
## PRIMARY KEY

```sql
CREATE TABLE Persons (
    ID int NOT NULL PRIMARY KEY,
    LastName varchar(255) NOT NULL,
    FirstName varchar(255),
    Age int
);

ALTER TABLE Persons
ADD PRIMARY KEY (ID);

ALTER TABLE Persons
ADD CONSTRAINT PK_Person PRIMARY KEY (ID,LastName);


ALTER TABLE Persons
DROP PRIMARY KEY;

ALTER TABLE Persons
DROP CONSTRAINT PK_Person;
```

## FOREIGN KEY
```sql
CREATE TABLE Orders (
    OrderID int NOT NULL,
    OrderNumber int NOT NULL,
    PersonID int,
    PRIMARY KEY (OrderID),
    FOREIGN KEY (PersonID) REFERENCES Persons(PersonID)
);

ALTER TABLE Orders
ADD FOREIGN KEY (PersonID) REFERENCES Persons(PersonID);

ALTER TABLE Orders
ADD CONSTRAINT FK_PersonOrder
FOREIGN KEY (PersonID) REFERENCES Persons(PersonID);
```

## CHECK
```sql
CREATE TABLE Persons (
    ID int NOT NULL,
    LastName varchar(255) NOT NULL,
    FirstName varchar(255),
    Age int,
    CHECK (Age>=18)
);

ALTER TABLE Persons
ADD CHECK (Age>=18);

ALTER TABLE Persons
ADD CONSTRAINT CHK_PersonAge CHECK (Age>=18 AND City='Sandnes');

```

## DEFAULT
```sql
CREATE TABLE Persons (
    ID int NOT NULL,
    LastName varchar(255) NOT NULL,
    FirstName varchar(255),
    Age int,
    City varchar(255) DEFAULT 'Sandnes'
);

ALTER TABLE Persons
ALTER City SET DEFAULT 'Sandnes';

ALTER TABLE Persons
ADD CONSTRAINT df_City
DEFAULT 'Sandnes' FOR City;

```

## INDEX
```sql
CREATE UNIQUE INDEX index_name
ON table_name (column1, column2, ...);
```

## AUTO INCREMENT
```sql
CREATE TABLE Persons (
    Personid int NOT NULL AUTO_INCREMENT,
    LastName varchar(255) NOT NULL,
    FirstName varchar(255),
    Age int,
    PRIMARY KEY (Personid)
);
```

°°°
Count from 100

```sql
ALTER TABLE Persons AUTO_INCREMENT=100;

```


## VIEW

```sql
CREATE VIEW [Brazil Customers] AS
SELECT CustomerName, ContactName
FROM Customers
WHERE Country = 'Brazil';
```

°°°
Update

```sql
CREATE OR REPLACE VIEW [Brazil Customers] AS
SELECT CustomerName, ContactName, City
FROM Customers
WHERE Country = 'Brazil';
```

## 3 types of Commands
* DDL
* DML
* DCL

## DDL
* CREATE
* ALTER
* DROP


## Date and Time

- Dates: 'YYYY MM DD' e.g. '1975 05 17'
- Times: ‘hh:mm:ss[.f] ' e.g. '15:00:00'
- Timestamp: ‘YYYY MM DD hh:mm:ss[.f] ' e.g. ‘1975 05 17 15:00:00'

## To add date
```sql
DATE_ADD(date, INTERVAL expr unit)
```

- date: The starting date
- expr: The value of the time interval to add
- unit: The unit of the time interval (e.g., DAY, MONTH, YEAR)


## CREATE DOMAIN

The CREATE DOMAIN command allows you to define your own types that are subsets of built in types:

```sql
CREATE DOMAIN
domainName AS dataType
[DEFAULT defaultValue]
[CHECK (condition)]

CREATE DOMAIN
titleType AS CHAR(2)
DEFAULT 'EE'
CHECK (VALUE IN
(NULL,'EE','SA','PR','ME'))
```

## SQL Referential Integrity & Updates

When you try to INSERT or UPDATE a row in a relation containing a foreign key , that operation is rejected if it violates referential integrity. 
When you UPDATE or DELETE a row in the primary key relation, you have the option on what happens to the values in the foreign key relation.

* **CASCADE** Delete (update) values in foreign key relation when primary key relation has rows deleted (updated).
* **SET NULL** Set foreign key fields to NULL when corresponding primary key relation row is deleted.
* **SET DEFAULT** Set foreign key values to their default value (if defined).
* **NO ACTION** Reject the request on the parent table *MySQL equivalent is RESTRICT


```sql
FOREIGN KEY (dno) REFERENCES Dept(dno)
ON DELETE SET NULL ON UPDATE CASCADE
```

## ALTER
```sql
ALTER TABLE table_name ADD column_name datatype
ALTER TABLE table_name DROP COLUMN column_name
ALTER TABLE table_name MODIFY COLUMN column_name datatype
ALTER TABLE table_name ADD CONSTRAINT constraint( column_name)
```

## INDEX

```sql
CREATE INDEX index_name ON table_name column1
ALTER TABLE table_name DROP INDEX index_name
```

## Trigger
A trigger is a set of actions that are run automatically when a specified change operation (SQL INSERT, UPDATE, or DELETE statement) is performed on a specified table.

EXAMPLE
```sql
CREATE TABLE people (age INT, name varchar(150));

CREATE TRIGGER agecheck BEFORE INSERT ON people FOR EACH ROW IF NEW.age < 0 THEN SET NEW.age = 0; END IF

INSERT INTO people VALUES 20, ‘Sid’), (30, ‘Josh’);
```

## TRANSACTION
A transaction is a logical unit of work that contains one or more SQL statements.

1. either all the operations in the transaction are completed successfully and their effect is recorded permanently in the database
2. or that the transaction does not have any effect on the database or any other transactions.

Properties
* ATOMICITY
* CONSISTENCY
   Database properly change state after successful transaction
* ISOLATION
   Independent Transactions
* DURABILITY
   Effect Persist even after system failure

Modes
By default, MySQL runs with autocommit mode enabled
```sql
SET AUTOCOMMIT = 0;
```

## TRANSACTION SYNTAX

```sql
DECLARE @TranName VARCHAR(20);  
SELECT @TranName = 'MyTransaction';  
  
BEGIN TRANSACTION @TranName;  
USE AdventureWorks2012;  
DELETE FROM AdventureWorks2012.HumanResources.JobCandidate  
    WHERE JobCandidateID = 13;  
  
COMMIT TRANSACTION @TranName;  
GO
```

## SAVEPOINT and ROLLBACK

```sql
SQL> SAVEPOINT SP1;
Savepoint created.
SQL> DELETE FROM CUSTOMERS WHERE ID=1;
1 row deleted.
SQL> SAVEPOINT SP2;
Savepoint created.
SQL> DELETE FROM CUSTOMERS WHERE ID=2;
1 row deleted.
SQL> SAVEPOINT SP3;
Savepoint created.
SQL> DELETE FROM CUSTOMERS WHERE ID=3;
1 row deleted.

SQL> ROLLBACK TO SP2;
Rollback complete.4
```

**The RELEASE SAVEPOINT command is used to remove a SAVEPOINT that you have created.**
```sql
RELEASE SAVEPOINT SAVEPOINT_NAME;
```

## UPDATE

```sql

UPDATE table_name
SET column1 = value1, column2 = value2...., columnN = valueN
WHERE [condition];
```

## PRIVILEGES
```sql
GRANT SELECT, INSERT, UPDATE, DELETE ON SUPPLIER TO user1
GRANT SELECT (PRODNR, PRODNAME) ON PRODUCT TO user1
REVOKE DELETE ON SUPPLIER FROM user1
```

## ROUND

ROUND

- ROUND(f,p) returns f rounded to p decimal places.

```sql
SELECT name,
       ROUND(population/1000000,1)
  FROM bbc

```

The number of decimal places may be negative, this will round to the nearest 10 (when p is -1) or 100 (when p is -2) or 1000 (when p is -3) etc

```sql
-- 7254
ROUND(7253.86, 0)


-- 7253.9
ROUND(7253.86, 1)


-- 7000
ROUND(7253.86,-3)
```



## LENGTH

```sql
SELECT LENGTH(name), name
  FROM bbc
```

## LEFT

- `LEFT(s,n)` allows you to extract n characters from the start of the string s.

```sql
LEFT('Hello world', 4)
-- 'Hell' 
```

## Correlated Subquery

Find the largest country (by area) in each continent, show the continent, the name and the area:

```sql
SELECT w1.continent, name, w1.area 
  FROM world AS w1
  JOIN (SELECT continent, MAX(area) AS area
          FROM world 
         GROUP BY continent) AS w2
    ON w1.continent = w2.continent
   AND w1.area = w2.area




SELECT x.continent, x.name, x.area
FROM world AS x
WHERE x.area = (
  SELECT MAX(y.area)
  FROM world AS y
  WHERE x.continent = y.continent)
```


## Position of Having

```sql
SELECT column_name(s)
FROM table_name
WHERE condition
GROUP BY column_name(s)
HAVING condition
ORDER BY column_name(s)
LIMIT
OFFSET;
```

## Drop 
```sql
Drop Table table_name;
```

## Use NULL


MySQL uses three-valued logic -- TRUE, FALSE and UNKNOWN. Anything compared to NULL evaluates to the third value: UNKNOWN. That “anything” includes NULL itself! That’s why MySQL provides the IS NULL and IS NOT NULL operators to specifically check for NULL.



Find the names of the customer that are not referred by the customer with id = 2.

```sql
--  WRONG
SELECT name FROM customer WHERE referee_Id <> 2;
```

> Customers who visited but didn't make any transaction

```sql
SELECT 
  customer_id, 
  COUNT(*) AS count_no_trans 
FROM 
  Visits AS v 
  LEFT JOIN Transactions AS t ON v.visit_id = t.visit_id 
WHERE 
  t.visit_id IS NULL 
GROUP BY 
  customer_id
```


## offset

OFFSET dictates the number of rows to skip from the beginning of the returned data before presenting the results.

```sql
SELECT 
    column_list
FROM
    table1
ORDER BY column_list
LIMIT row_count OFFSET offset;
```


## CTE

A Common Table Expression (CTE) is the result set of a query which exists temporarily and for use only within the context of a larger query. Much like a derived table, the result of a CTE is not stored and exists only for the duration of the query.

```sql
WITH my_cte AS (
  SELECT a,b,c
  FROM T1
)
SELECT a,c
FROM my_cte
WHERE ....
```

## Why Columnar Databases are faster for retrieval

Essentially, the main difference between row oriented and column oriented DBs is the model they use to serialize data. Row oriented DBs store the data in each row as contiguous blocks. Column oriented DBs store the data of each column in contiguous blocks. Further, those blocks are typically compressed and sorted.

So, the difference in performance really depends on the type of query. Queries that use less I/O seeks will perform faster and reading from a contiguous block is a single seek. So if your query relies on aggregations or sorting on a column (or multiple columns) then a column store can perform much faster because reading all values in the column can be a single seek under optimal conditions. If your query is searching for a handful of customer records in a huge customer table based on an indexed column like a customer ID then a row store DB might actually be faster.

## Sharding 
Sharding is a very important concept that helps the system to keep data in different resources according to the sharding process. The word “Shard” means “a small part of a whole“. Hence Sharding means dividing a larger part into smaller parts. In DBMS, Sharding is a type of DataBase partitioning in which a large database is divided or partitioned into smaller data and different nodes. These shards are not only smaller, but also faster and hence easily manageable. 

**Need for Sharding:**  
Consider a very large database whose sharding has not been done. For example, let’s take a DataBase of a college in which all the student’s records (present and past) in the whole college are maintained in a single database. So, it would contain a very very large number of data, say 100, 000 records. Now when we need to find a student from this Database, each time around 100, 000 transactions have to be done to find the student, which is very very costly. Now consider the same college students records, divided into smaller data shards based on years. Now each data shard will have around 1000-5000 students records only. So not only the database became much more manageable, but also the transaction cost each time also reduces by a huge factor, which is achieved by Sharding. Hence this is why Sharding is needed. 

**How does Sharding work?**  
In a sharded system, the data is partitioned into shards based on a predetermined criterion. For example, a sharding scheme may divide the data based on geographic location, user ID, or time period. Once the data is partitioned, it is distributed across multiple servers or nodes. Each server or node is responsible for storing and processing a subset of the data.

To query data from a sharded database, the system needs to know which shard contains the required data. This is achieved using a shard key, which is a unique identifier that is used to map the data to its corresponding shard. When a query is received, the system uses the shard key to determine which shard contains the required data and then sends the query to the appropriate server or node.

## Index

Indexes in SQL: A Comprehensive Tutorial

Introduction:
Indexes are a crucial performance-tuning method in SQL databases. They enable faster data retrieval, improving query efficiency. In this tutorial, we'll delve into the world of indexes, exploring what they are, types, benefits, and how to create and manage them.

What are Indexes in SQL?
An index is a data structure that improves query performance by providing quick access to specific data. It's similar to a book's index, where you can find specific information quickly. Indexes contain a copy of selected columns and corresponding row locations, allowing the database to bypass scanning the entire table.

Types of Indexes:

1. B-Tree Index: The most common index type, using a balanced tree structure for efficient data retrieval.
2. Hash Index: Optimized for queries using the = operator, using a hash table to store data.
3. Full-Text Index: Designed for searching text data, allowing for efficient full-text searches.
4. Composite Index: Covers multiple columns, improving queries that filter on those columns.
5. Unique Index: Ensures data uniqueness in a column or set of columns.
6. Clustered Index: Reorders physical data to match the index, improving range queries.

Benefits of Indexes:

1. Faster Query Performance: Indexes reduce the time it takes to retrieve data.
2. Improved Data Retrieval: Indexes enable the database to locate data quickly.
3. Reduced Disk I/O: By minimizing data scanning, indexes reduce disk I/O operations.

Creating Indexes:

1. CREATE INDEX: The basic syntax for creating an index.

CREATE INDEX index_name ON table_name (column_name);

1. CREATE UNIQUE INDEX: Creates a unique index, ensuring data uniqueness.

CREATE UNIQUE INDEX index_name ON table_name (column_name);

1. CREATE COMPOSITE INDEX: Covers multiple columns.

CREATE INDEX index_name ON table_name (column_name1, column_name2);

Managing Indexes:

1. DROP INDEX: Deletes an index.

DROP INDEX index_name;

1. ALTER INDEX: Modifies an existing index.

ALTER INDEX index_name REBUILD;

1. INDEX REBUILD: Rebuilds an index to maintain performance.

ALTER INDEX index_name REBUILD;

Best Practices:

1. Index Frequently Used Columns: Index columns used in WHERE, JOIN, and ORDER BY clauses.
2. Avoid Over-Indexing: Too many indexes can slow down writes and waste space.
3. Monitor Index Performance: Regularly analyze index usage and adjust as needed.

Conclusion:
Indexes are a powerful tool for improving SQL query performance. By understanding the different types, benefits, and management techniques, you'll be able to optimize your database for faster data retrieval and improved overall performance. Remember to index wisely and monitor performance to ensure optimal database operation.

## View

A view in SQL is a virtual table that is based on the result of a SELECT statement. It does not store data itself but provides a way to simplify complex queries and present data in a more organized way.

A view can be thought of as a stored query that can be queried like a physical table. When a view is queried, the database engine executes the underlying SELECT statement and returns the result set.

Views are useful for several reasons:

1. Simplifying complex queries: Views can hide the complexity of a query and present a simpler interface to the user.
2. Data abstraction: Views can abstract away the underlying table structure and present data in a more organized way.
3. Data security: Views can be used to restrict access to certain data by limiting the columns or rows that are visible.
4. Improved performance: Views can improve performance by reducing the number of queries needed to retrieve data.

A view is created using the CREATE VIEW statement, followed by the name of the view and the SELECT statement that defines the view.

For example:

CREATE VIEW customer_addresses AS
SELECT c.customer_id, c.name, a.address, a.city, a.state, a.zip
FROM customers c
JOIN addresses a ON c.customer_id = a.customer_id;

Once a view is created, it can be queried like a physical table:

SELECT * FROM customer_addresses;

Views can be used in various ways, such as:

1. Selecting data: Views can be used to retrieve data from multiple tables in a single query.
2. Inserting data: Views can be used to insert data into multiple tables with a single statement.
3. Updating data: Views can be used to update data in multiple tables with a single statement.
4. Deleting data: Views can be used to delete data from multiple tables with a single statement.

However, views have some limitations, such as:

1. Data modification: Views can be used to modify data, but the modifications are not stored in the view itself.
2. Data consistency: Views can become outdated if the underlying data changes.
3. Performance: Views can impact performance if they are not optimized properly.

Overall, views are a powerful tool in SQL that can simplify complex queries, abstract away data, and improve performance. However, they should be used judiciously and with caution to avoid potential issues.


## Is View just a stored query or the is it the stored data from query?

A view is a stored query, not stored data. When you create a view, you are essentially storing a SQL query that can be executed later. The data is not stored in the view itself, but rather the view provides a way to access the data in the underlying tables.

When you query a view, the database engine executes the stored query and returns the result set, which is derived from the data in the underlying tables. The data is not cached or stored in the view, so the view always reflects the current state of the data in the underlying tables.

In other words, a view is a way to encapsulate a complex query and present it as a single, simplified table-like interface, but it does not store any data itself. The data is still stored in the underlying tables, and the view is just a way to access and manipulate that data.

This is in contrast to a materialized view, which is a type of view that actually stores the result set of the query in a physical table. Materialized views are typically used in data warehousing and business intelligence applications where the data is relatively static and the queries are complex and resource-intensive.

So, to summarize, a view is a stored query that provides a way to access data in underlying tables, but it does not store any data itself.

## If view is not stored data and just a query then how can it speed up the data retrieval?

While a view is just a stored query and doesn't store data, it can still speed up data retrieval in several ways:

1. Query optimization: When you create a view, the database engine optimizes the query that defines the view. This means that the query is analyzed, and an execution plan is created to retrieve the data as efficiently as possible. When you query the view, the optimized execution plan is used, which can lead to faster data retrieval.
2. Caching: Some databases, like Oracle, cache the results of a view query in memory. This means that if the data in the underlying tables hasn't changed, the database can return the cached results instead of re-executing the query. This can lead to significant performance improvements.
3. Reduced complexity: Views can simplify complex queries, making it easier for the database engine to execute them. By breaking down a complex query into smaller, more manageable pieces, a view can reduce the overhead of query execution.
4. Indexing: In some cases, a view can be indexed, just like a physical table. This allows the database engine to use indexes to quickly locate the data, leading to faster query performance.
5. Data pruning: When you query a view, the database engine only needs to access the data that's relevant to the view's query. This can reduce the amount of data that needs to be read, leading to faster query performance.

While a view doesn't store data, these factors can still contribute to faster data retrieval. However, it's important to note that views can also introduce additional overhead, such as the cost of maintaining the view's metadata and executing the view's query. So, it's essential to carefully consider the trade-offs when using views in your database design.


## Columnar Databases

A columnar database is a type of database management system (DBMS) that stores data in columns rather than rows, which can result in more efficient access to data when only querying a subset of columns ¹ ² ³. Columnar databases are well-suited for data warehousing, business intelligence and analytics workloads because of the large dataset sizes, query types, and low update frequency ¹.

## Normalization

Normalization in SQL is like cleaning up your closet!

Imagine you have a closet where you keep all your clothes, shoes, and accessories. At first, it's easy to find what you need, but as you add more stuff, it becomes cluttered and hard to navigate.

In a database, normalization is the process of organizing data in a way that:

1. Eliminates redundant data (like having multiple copies of the same shirt)
2. Reduces data dependencies (like keeping shoes and clothes in separate sections)
3. Improves data integrity (like making sure each item has a clear label)

Here's a simple example:

Let's say you have a table called "Customers" with columns like "Name", "Address", "Phone Number", and "Order History". As you add more customers, the table becomes cluttered, and it's hard to update or delete data without causing errors.

To normalize the table, you would:

1. Create separate tables for "Customers", "Addresses", and "Orders"
2. Link the tables using unique IDs (like a customer ID)
3. Move the relevant data to the corresponding tables (e.g., move the address data to the "Addresses" table)

Now, each table has a clear purpose, and updating or deleting data is much easier and safer!

That's normalization in a nutshell!

## 2NF

The second normal form (2NF) is a principle in database normalization that eliminates partial dependencies on primary keys. A table is in 2NF if it meets the following criteria ¹ ² ³ ⁴ ⁵:

1. It is in 1NF.
2. It does not have any non-prime attribute that is functionally dependent on any proper subset of any candidate key of the relation.
3. Every non-key attribute is fully dependent on the primary key.
4. There are no partial dependencies on the primary key.

## Partial dependency

A partial dependency on a primary key occurs when a non-key attribute (a column that is not part of the primary key) depends on only one part of the primary key.

Think of it like a combination lock. The primary key is like the combination, and the non-key attributes are like the treasure inside. If the treasure (non-key attribute) can be accessed by only one number (part of the primary key), it's a partial dependency.

For example, consider a table with the following columns:

- EmployeeID (primary key)
- DepartmentID (primary key)
- EmployeeName
- DepartmentName

In this table, EmployeeName depends on EmployeeID, which is only one part of the primary key. This is a partial dependency because EmployeeName should depend on the entire primary key (EmployeeID and DepartmentID).

To fix this, you would split the table into two separate tables:

- Employees (EmployeeID, EmployeeName)
- Departments (DepartmentID, DepartmentName)

Now, EmployeeName depends on the entire primary key (EmployeeID) in the Employees table, and DepartmentName depends on the entire primary key (DepartmentID) in the Departments table.

No more partial dependencies!

## 3NF

The third normal form (3NF) is a database schema design approach that uses normalizing principles to reduce data duplication, avoid data anomalies, ensure referential integrity and simplify data management ¹. A table is in 3NF if and only if the following conditions hold: the relation R is in second normal form (2NF) and no non-prime attribute of R is transitively dependent on the primary key ² ¹.

## Transitive dependency

Transitive dependency is a phenomenon where a non-key attribute (a column that is not part of the primary key) depends on another non-key attribute, which in turn depends on the primary key.

Think of it like a chain of dependencies:

Primary Key → Non-Key Attribute A → Non-Key Attribute B

In this chain, Non-Key Attribute B depends on Non-Key Attribute A, which depends on the Primary Key. This creates a transitive dependency, where Non-Key Attribute B indirectly depends on the Primary Key through Non-Key Attribute A.

For example, consider a table with the following columns:

- EmployeeID (primary key)
- DepartmentID (non-key attribute)
- DepartmentName (non-key attribute)

In this table, DepartmentName depends on DepartmentID, which in turn depends on EmployeeID. This creates a transitive dependency, as DepartmentName indirectly depends on EmployeeID through DepartmentID.

To eliminate transitive dependencies, you would split the table into separate tables, like:

- Employees (EmployeeID, DepartmentID)
- Departments (DepartmentID, DepartmentName)

Now, DepartmentName directly depends on DepartmentID, and there is no transitive dependency.


## 4NF

The fourth normal form (4NF) is a database normalization technique that builds upon the Boyce-Codd Normal Form (BCNF) by ensuring that a table does not contain any non-trivial multi-valued dependencies, except for candidate keys ¹ ². In other words, 4NF is concerned with a more general type of dependency known as a multi-valued dependency, where the presence of one value in a column depends on the presence of another value in another column. A table is in 4NF if and only if, for every non-trivial multi-valued dependency X Y, X is a superkey, which means that X is either a candidate key or a superset thereof.


## Non-trivial Multi-valued dependency

A non-trivial multi-valued dependency is a type of dependency that exists between two attributes in a table, where:

1. One attribute (X) determines the other attribute (Y)
2. X does not determine Y uniquely (i.e., multiple values of Y can be associated with a single value of X)
3. The dependency is not trivial, meaning that X is not a subset of Y or vice versa

In other words, a non-trivial multi-valued dependency exists when:

- X determines Y, but not uniquely (many-to-many relationship)
- X and Y are not identical or overlapping attributes

For example, consider a table with the following attributes:

- EmployeeID (X)
- Skill (Y)

In this table, EmployeeID determines Skill, but not uniquely, as an employee can have multiple skills. This is a non-trivial multi-valued dependency because EmployeeID does not uniquely determine Skill, and EmployeeID and Skill are not identical or overlapping attributes.

In 4NF, we aim to eliminate such non-trivial multi-valued dependencies by decomposing the table into separate tables, each with its own set of attributes that are dependent on a single key.

## Types of indexes

The different types of indexes in SQL include ¹ ²:
- Clustered Indexes: Clustered indexes store the index key and the actual table data in the leaf nodes of the index. A table can only have one clustered index.
- Non-Clustered Indexes: Non-clustered indexes store the index key in a B-tree structure, but the actual data is not stored in the leaf nodes. Instead, a pointer to the actual data is stored.
- Column Store Indexes: Column store indexes are a type of non-clustered index that use a column-based storage format to index data.
- XML Indexes: XML indexes are a special type of index that can be created on XML typed columns.
- Full-Text Indexes: Full-text indexes provide indexing support for full-text queries on binary or character-based column types.
- Included Columns Indexes: Included columns indexes are not a type of index, but rather a clause that can be added to a non-clustered index to store the column values in the leaf nodes of the index.
- Filtered Indexes: Filtered indexes are non-clustered indexes that include a WHERE clause to reduce the size of the index and improve query performance for specific queries.
- Covering Indexes: Covering indexes are non-clustered indexes where all columns referenced in a query are either part of the index key or specified in the included column clause.

## WINDOW FUNCTIONS

Here are some SQL window functions ¹ ² ³ ⁴:

- ROW_NUMBER: Assigns a unique number to each row within a partition of a result set.
- RANK: Assigns a rank to each row within a partition of a result set.
- DENSE_RANK: Similar to RANK, but assigns the same rank to tied rows and does not leave gaps in the ranking.
- LAG: Returns the value of a column from a previous row within a partition of a result set.
- LEAD: Similar to LAG, but returns the value of a column from a next row within a partition of a result set.
- SUM: Calculates the sum of a column within a partition of a result set.
- MAX: Returns the maximum value of a column within a partition of a result set.
- MIN: Returns the minimum value of a column within a partition of a result set.
- AVG: Calculates the average value of a column within a partition of a result set.
- COUNT: Counts the number of rows within a partition of a result set.

## Modules in DBMS
* Client Module
* Server Module

## Two Tier Architecture
* Client Module
* Server Module

## Three Tier
* Client
* Application Server
* Database Server

## Data Abstraction in Three Schema Architecture
* External Level
* Conceptual Level
* Internal Level

## Data Abstraction Leads to Data Independence
The capacity to change the schema at one level of a database
system without having to change the schema at the next higher
level.

* Logical Data Independence
* Physical Data Independence

## Schema
Description of Database

## Data Models
Collection of concepts that can be used to describe the structure of a database.

* Representational or Implementation data models
* Physical Data Models



## Relational Data Model
* Entity
* Attribute
* Relationship

A relation is a table with columns and rows.
An attribute is a named column of a relation.
A tuple is a row of a relation.
A domain is a set of allowable values for one or more attributes.
The degree of a relation is the number of attributes it contains.

The cardinality of a relation is the number of tuples it contains.
A relational database is a collection of normalized relations with distinct relation names.
The intension of a relation is the structure of the relation including its domains.
The extension of a relation is the set of tuples currently in the relation.

## Relational Constraints

> Domain Constraint
Atomic and single value from the domain dom(A)

> Key Constraint
A key that allows to uniquely identify its tuples

> Entity Integrity Constraint
Primary key should always satisfy a NOT NULL constraint

> Referential Integrity Constraint
- A foreign key FK has the same domain as the primary key PK attribute type(s) it refers to.
- Either occurs as a value of PK or NULL





# MUST SEE

## How to subtract 30 days from the current date using SQL Server

```sql
SELECT      GETDATE(), 'Today'
UNION ALL
SELECT      DATEADD(DAY,  10, GETDATE()), '10 Days Later'
UNION ALL
SELECT      DATEADD(DAY, –10, GETDATE()), '10 Days Earlier'
UNION ALL
SELECT      DATEADD(MONTH,  1, GETDATE()), 'Next Month'
UNION ALL
SELECT      DATEADD(MONTH, –1, GETDATE()), 'Previous Month'
UNION ALL
SELECT      DATEADD(YEAR,  1, GETDATE()), 'Next Year'
UNION ALL
SELECT      DATEADD(YEAR, –1, GETDATE()), 'Previous Year'
```

> User Activity for the Past 30 Days I MySql
```sql
with mycte as
(
select * from Activity
where activity_date <= date('2019-07-27') and activity_date > date_add(date('2019-07-27'), interval -30 day)
)
select activity_date day, count(distinct user_id) active_users from mycte
Group by activity_date

-- OR
SELECT activity_date AS day, COUNT(DISTINCT user_id) AS active_users
FROM Activity
WHERE (activity_date > "2019-06-27" AND activity_date <= "2019-07-27")
GROUP BY activity_date;
```

## managers with at least five direct reports.

+-------------+---------+
| Column Name | Type   |
+-------------+---------+
| id                     | int             |
| name              | varchar   |
| department | varchar   |
| managerId    | int            |
+-------------+---------+

```sql

SELECT e.name
FROM Employee AS e 
INNER JOIN Employee AS m ON e.id=m.managerId 
GROUP BY m.managerId 
HAVING COUNT(m.managerId) >= 5
```

## The Number of Employees Which Report to Each Employee

```
+-------------+----------+
| Column Name | Type     |
+-------------+----------+
| employee_id | int      |
| name        | varchar  |
| reports_to  | int      |
| age         | int      |
+-------------+----------+
employee_id is the column with unique values for this table.
This table contains information about the employees and the id of the manager they report to. Some employees do not report to anyone (reports_to is null). 
```

```sql
select mgr.employee_id, mgr.name, COUNT(emp.employee_id) as reports_count, ROUND(AVG(emp.age)) as average_age
from employees emp join employees mgr
on emp.reports_to = mgr.employee_id
group by employee_id
order by employee_id
```

## Compare consecutive rows of table

```
+-------------+---------+
| Column Name | Type    |
+-------------+---------+
| id          | int     |
| num         | varchar |
+-------------+---------+
In SQL, id is the primary key for this table.
id is an autoincrement column.
 

Find all numbers that appear at least three times consecutively.
```

> LEAD and LAG
```sql
Approach 1 -Using Joins
SELECT DISTINCT l1.num AS ConsecutiveNums
FROM Logs l1
JOIN Logs l2 ON l1.id = l2.id - 1
JOIN Logs l3 ON l1.id = l3.id - 2
WHERE l1.num = l2.num AND l2.num = l3.num;
```

```sql
#Approach 2-Using LAG and LEAD
WITH temporary_table(num, next_num, prev_num) AS (
    SELECT 
        num, 
        LEAD(num, 1, 0) OVER (ORDER BY id ASC) AS next_num,
        LAG(num, 1, 0) OVER (ORDER BY id ASC) AS prev_num 
    FROM Logs
)

SELECT DISTINCT num AS ConsecutiveNums 
FROM temporary_table 
WHERE num = next_num AND num = prev_num;
```

## Add a new column and its conditional  value

> Report for every three line segments whether they can form a triangle.
```sql
select x, y, z, 
case 
when
x+y > z and x+z > y and y+z > x
then 'Yes'
else 'No'
end
As triangle
from Triangle;


SELECT *, IF(x+y>z and y+z>x and z+x>y, "Yes", "No") as triangle FROM Triangle
```

## Add a column with Running aggregate

> Last Person to Fit in the Bus

```sql
+-------------+---------+
| Column Name | Type    |
+-------------+---------+
| person_id   | int     |
| person_name | varchar |
| weight      | int     |
| turn        | int     |
+-------------+---------+
person_id column contains unique values.
This table has the information about all people waiting for a bus.
The person_id and turn columns will contain all numbers from 1 to n, where n is the number of rows in the table.
turn determines the order of which the people will board the bus, where turn=1 denotes the first person to board and turn=n denotes the last person to board.
weight is the weight of the person in kilograms.
```

```sql
with running_weight as(
            select *,
                SUM(weight) OVER(order by turn) as running_wt
            from Queue
) select person_name
  from running_weight
  where running_wt <= 1000
  order by running_wt desc
  limit 1;
```

## FETCH AND OFFSET

> Second highest salary

```
+-------------+------+
| Column Name | Type |
+-------------+------+
| id          | int  |
| salary      | int  |
+-------------+------+
id is the primary key (column with unique values) for this table.
Each row of this table contains information about the salary of an employee.
```

```sql
select salary as SecondHighestSalary from Employee
order by salary desc
offset 1 ROW
fetch next 1 rows only
```




> Without offset

```sql
/* Write your T-SQL query statement below */
select max(salary) SecondHighestSalary from Employee where salary <> (select max(salary) from employee)
```

### Conditional rendering of values of a column

```sql
SELECT 
    IF(
        (SELECT COUNT(*) FROM employee) = 1,
        NULL,
        (
            SELECT 
                DISTINCT salary 
            FROM 
                employee
            WHERE salary < (SELECT MAX(salary) FROM employee)
            ORDER BY salary DESC
            LIMIT 1
        )
    )AS SecondHighestSalary;

```

## Delete Duplicate Emails

```
+-------------+---------+
| Column Name | Type    |
+-------------+---------+
| id          | int     |
| email       | varchar |
+-------------+---------+
id is the primary key (column with unique values) for this table.
Each row of this table contains an email. The emails will not contain uppercase letters.
```

```sql
DELETE p1 FROM Person p1,
    Person p2
WHERE
    p1.Email = p2.Email AND p1.Id > p2.Id
```

```sql
delete from cars
where model_id not in (select min(model_id)
					  from cars
					  group by model_name, brand);
```

## Summary creation of category

```
+-------------+------+
| Column Name | Type |
+-------------+------+
| account_id  | int  |
| income      | int  |
+-------------+------+
account_id is the primary key (column with unique values) for this table.
Each row contains information about the monthly income for one bank account.
 

Write a solution to calculate the number of bank accounts for each salary category. The salary categories are:

"Low Salary": All the salaries strictly less than $20000.
"Average Salary": All the salaries in the inclusive range [$20000, $50000].
"High Salary": All the salaries strictly greater than $50000.
The result table must contain all three categories. If there are no accounts in a category, return 0.

Return the result table in any order.
```


> Wrong Code: BC if there is no salary in the given category then there won't be that category in the summary table
```sql
with mycte as
(
select *,
case
when income < 20000 then "Low Salary"
when income >= 20000 and income <=50000 then "Average Salary"
else "High Salary"
end AS category
from Accounts
)
select category, count(*) as accounts_count
from mycte group by category
```

> Correct Code

```sql
# Write your MySQL query statement below
SELECT 
    'Low Salary' AS category,
    SUM(income < 20000) AS accounts_count
FROM 
    Accounts

UNION 

    SELECT 
        'Average Salary' AS category,
        SUM(income BETWEEN 20000 AND 50000 ) AS accounts_count
    FROM 
        Accounts

UNION

    SELECT 
        'High Salary' AS category,
        SUM(income > 50000) AS accounts_count
    FROM 
        Accounts;
```


## Write a solution to report the movies with an odd-numbered ID and a description that is not "boring".

```sql

select * from Cinema
where description != 'boring' and id%2 <> 0 order by rating desc;



SELECT * FROM Cinema
WHERE MOD(id, 2) <> 0 AND description <> 'boring'
ORDER BY rating DESC
```

## Write a solution to find all dates' Id with higher temperatures compared to its previous dates (yesterday).


```sql
select distinct id from Weather as w1 where w1.temperature > (select temperature from Weather w2 where DATEDIFF(w1.recordDate, w2.recordDate) = 1);



SELECT 
    w1.id
FROM 
    Weather w1
JOIN 
    Weather w2
ON 
    DATEDIFF(w1.recordDate, w2.recordDate) = 1
WHERE 
    w1.temperature > w2.temperature;
```

## 
The resulting table should have the machine_id along with the average time as processing_time, which should be rounded to 3 decimal places.



+----------------+---------+
| Column Name| Type |
+----------------+---------+
| machine_id     | int      |
| process_id      | int      |
| activity_type  | enum|
| timestamp      | float  |
+----------------+---------+


`The table shows the user activities for a factory website.
(machine_id, process_id, activity_type) is the primary key (combination of columns with unique values) of this table.
machine_id is the ID of a machine.
process_id is the ID of a process running on the machine with ID machine_id.
activity_type is an ENUM (category) of type ('start', 'end').
timestamp is a float representing the current time in seconds.
'start' means the machine starts the process at the given timestamp and 'end' means the machine ends the process at the given timestamp.
The 'start' timestamp will always be before the 'end' timestamp for every (machine_id, process_id) pair.`


The resulting table should have the machine_id along with the average time as processing_time, which should be rounded to 3 decimal places.

```sql
select a1.machine_id, 
ROUND(AVG(a2.timestamp-a1.timestamp),3)
as processing_time from Activity a1
join Activity a2
on 
a1.machine_id = a2.machine_id and
a1.process_id = a2.process_id and
a1.activity_type <> a2.activity_type and
a1.timestamp < a2.timestamp
Group by machine_id;

```
## NOTE

```sql
SELECT name,
CONCAT(
ROUND(
100*population/
(SELECT population from world where name='Germany'))
, '%')
FROM world
where continent='Europe'
```

## Note

```sql
Select name from world
Where 
name like '%a' 
OR 
name like '%l'
```

## Order By with CASE

Show the 1984 winners and subject ordered by subject and winner name; but list chemistry and physics last.

```sql
SELECT winner, subject
FROM nobel
WHERE yr=1984
ORDER BY 
CASE WHEN subject IN ('physics', 'chemistry')
THEN 1
ELSE 0
END, subject, winner
```


## VV IMP

For every match involving 'POL', show the matchid, date and the number of goals scored.


```sql
SELECT matchid, mdate, COUNT(*)
FROM goal JOIN game ON matchid = id 
WHERE (team1 = 'POL' OR team2 = 'POL')
GROUP BY matchid, mdate



SELECT matchid, mdate, COUNT(player)
FROM goal JOIN
     game
     ON matchid = id
WHERE 'POL' IN (team1, team2)
GROUP BY matchid, mdate;

```

## VV IMP: CASE IN SELECT

-- 13. List every match with the goals scored by each team as shown.
-- Sort your result by mdate, matchid, team1 and team2.


```sql
SELECT mdate,
  team1,
  SUM(CASE WHEN teamid=team1 THEN 1 ELSE 0 END) score1,
  team2,
  SUM(CASE WHEN teamid=team2 THEN 1 ELSE 0 END) score2
FROM game JOIN goal ON goal.matchid = game.id
GROUP BY game.id
ORDER BY mdate, matchid, team1, team2

```


## query quality

+-------------+---------+
| Column Name | Type    |
+-------------+---------+
| query_name  | varchar |
| result               | varchar |
| position          | int     |
| rating              | int     |
+-------------+---------+


This table may have duplicate rows.
This table contains information collected from some queries on a database.
The position column has a value from 1 to 500.
The rating column has a value from 1 to 5. Query with rating less than 3 is a poor query.


We define query quality as:

The average of the ratio between query rating and its position.

We also define poor query percentage as:

The percentage of all queries with rating less than 3.

Write a solution to find each query_name, the quality and poor_query_percentage

```sql
select
query_name,
round(avg(cast(rating as decimal) / position), 2) as quality,
round(sum(case when rating < 3 then 1 else 0 end) * 100 / count(*), 2) as poor_query_percentage
from
queries
where query_name is  not null
group by
query_name;
```















# Example

## XOR

Show the countries that are big by area (more than 3 million) or big by population (more than 250 million) but not both

```sql
SELECT name
    , population
    , area
FROM world
WHERE (area > 3000000 AND population <= 250000000)
OR (area <= 3000000 AND population > 250000000)
```


## Order By Multiple Cols

List the winners, year and subject where the winner starts with Sir. Show the the most recent first, then by name order.
```sql
select winner, yr, subject from nobel where winner LIKE 'Sir%' Order By yr DESC, winner ASC

```

## Bypass Null

Which countries have a GDP greater than every country in Europe? [Give the name only.] (Some countries may have NULL gdp values)
```sql
SELECT name FROM world WHERE gdp > ALL(SELECT gdp FROM world WHERE gdp > 0 AND continent = 'Europe');
```


## List each continent and the name of the country that comes first alphabetically.

```sql
Select  x.continent, x.name
From world x
Where x.name <= ALL (select y.name from world y where x.continent=y.continent)
ORDER BY name
```

## Group By and Having

List the continents that have a total population of at least 100 million.

```sql
SELECT continent
FROM world
GROUP BY continent
HAVING SUM(population) >= 100000000;
```

## See

movie:
id | title | yr | director | budget | gross

actor:
id | name

casting:
movieid | actorid | ord


Obtain a list, in alphabetical order, of actors who've had at least 15 starring roles

```sql
select actor.name
 from casting 
 join actor
on actor.id = casting.actorid
where ord = 1
group by actor.name
having count(ord) >= 15

```

List all the people who have worked with 'Art Garfunkel'

```sql
select distinct actor.name
from casting
join actor on casting.actorid = actor.id
where casting.movieid in (select casting.movieid
                           from casting
                           join actor on casting.actorid = actor.id
                           where actor.name = 'Art Garfunkel')
and actor.name != 'Art Garfunkel'
order by actor.name;
```












# Misc
## HAVING vs WHERE
A HAVING clause is like a WHERE clause, but applies only to groups as a whole (that is, to the rows in the result set representing groups), whereas the WHERE clause applies to individual rows.

## How to make stored Procedures

- [javatpoint.com](https://www.javatpoint.com/stored-procedure-in-sql-server)

## What are the differences between PRIMARY, UNIQUE, INDEX and FULLTEXT when creating MySQL tables?

### Differences

 - **KEY** or **INDEX** refers to a normal non-unique index.  Non-distinct values for the index are allowed, so the index *may* contain rows with identical values in all columns of the index.  These indexes don't enforce any restraints on your data so they are used only for access - for quickly reaching certain ranges of records without scanning all records.

 - **UNIQUE** refers to an index where all rows of the index must be unique.  That is, the same row may not have identical non-NULL values for all columns in this index as another row.  As well as being used to quickly reach certain record ranges, UNIQUE indexes can be used to enforce restraints on data, because the database system does not allow the distinct values rule to be broken when inserting or updating data.

   Your database system may allow a UNIQUE index to be applied to columns which allow NULL values, in which case two rows are allowed to be identical if they both contain a NULL value (the rationale here is that NULL is considered not equal to itself).  Depending on your application, however, you *may* find this undesirable: if you wish to prevent this, you should disallow NULL values in the relevant columns.

 - **PRIMARY** acts exactly like a UNIQUE index, except that it is always named 'PRIMARY', and there may be only one on a table (and there *should* always be one; though some database systems don't enforce this).  A PRIMARY index is intended as a primary means to uniquely identify any row in the table, so unlike UNIQUE it should not be used on any columns which allow NULL values.  Your PRIMARY index should be on the smallest number of columns that are sufficient to uniquely identify a row.  Often, this is just one column containing a unique auto-incremented number, but if there is anything else that can uniquely identify a row, such as "countrycode" in a list of countries, you can use that instead.

   Some database systems (such as MySQL's InnoDB) will store a table's records on disk in the order in which they appear in the PRIMARY index.

 - **FULLTEXT** indexes are different from all of the above, and their behaviour differs significantly between database systems.  FULLTEXT indexes are only useful for full text searches done with the MATCH() / AGAINST() clause, unlike the above three - which are typically implemented internally using b-trees (allowing for selecting, sorting or ranges starting from left most column) or hash tables (allowing for selection starting from left most column).

   Where the other index types are general-purpose, a FULLTEXT index is specialised, in that it serves a narrow purpose: it's only used for a "full text search" feature.

### Similarities

 - All of these indexes may have more than one column in them.

 - With the exception of FULLTEXT, the column order is significant: for the index to be useful in a query, the query must use columns from the index starting from the left - it can't use just the second, third or fourth part of an index, unless it is also using the previous columns in the index to match static values.  (For a FULLTEXT index to be useful to a query, the query must use *all* columns of the index.)

# functions

## SUBSTRING

```sql
SUBSTRING(string, start, length)

-- length
-- The start position. The first position in string is 1
```

## LEAD and LAG

```
LEAD(expr, N, default) 
          OVER (Window_specification | Window_name)
```

- **expr**: It can be a column or any built-in function.
- **N**: It is a positive value which determine number of rows preceding/succeeding the current row. If it is omitted in query then its default value is 1.
- **default**: It is the default value return by function in-case no row precedes/succeedes the current row by N rows. If it is missing then it is by default NULL.
- **OVER()**: It defines how rows are partitioned into groups. If OVER() is empty then function compute result using all rows.
- **Window_specification**: It consist of query partition clause which determines how the query rows are partitioned and ordered.
- **Window_name**: If window is specified elsewhere in the query then it is referenced using this Window_name.



# WINDOW FUNCTIONS 

## Link
- [sql](https://learnsql.com/blog/sql-window-functions-practice-exercises/)

## Dataset
- The `customer` table stores information on all registered customers. The columns are `id`, `first_name`, `last_name`, `join_date`, and `country`.
- The `movie` table contains records of all movies available in the store. The columns are `id`, `title`, `release_year`, `genre`, and `editor_ranking`.
- The `review` table stores customer ratings of the movies. The columns are `id`, `rating`, `customer_id` (references the `customer` table), and `movie_id` (references the `movie` table).
- The `single_rental` table stores information about movies that were rented for a certain period of time by customers. The columns are `id`, `rental_date`, `rental_period`, `platform`, `customer_id` (references the `customer` table), `movie_id` (references the `movie` table), `payment_date`, and `payment_amount`.
- The `subscription` table stores records for all customers who subscribed to the store. The columns are `id`, `length` (in days), `start_date`, `platform`, `payment_date`, `payment_amount`, and `customer_id` (references the `customer` table).
- The `giftcard` table contains information about purchased gift cards. The columns are `id`, `amount_worth`, `customer_id` (references the `customer` table), `payment_date`, and `payment_amount`.


### Rank Rentals by Price
For each single rental, show the `rental_date`, the title of the movie rented, its genre, the payment amount, and the rank of the rental in terms of the price paid (the most expensive rental should have rank = 1). The ranking should be created separately for each movie genre. Allow the same rank for multiple rows and allow gaps in numbering.

```sql
SELECT
  rental_date,
  title,
  genre,
  payment_amount,
  RANK() OVER(PARTITION BY genre ORDER BY payment_amount DESC)
FROM movie
JOIN single_rental
  ON single_rental.movie_id = movie.id;
```

> As the ranking should be created separately for each movie genre, in the OVER() clause, we partition the data by the genre column.

### Find 2nd Giftcard-Purchasing Customer
Show the first and last name of the customer who bought the second most-recent gift card, along with the date when the payment took place. Assume that a unique rank is assigned for each gift card purchase.

```sql
WITH ranking AS (
  SELECT
    first_name,
    last_name,
    payment_date,
    ROW_NUMBER() OVER(ORDER BY payment_date DESC) AS rank
  FROM customer
  JOIN giftcard
    ON customer.id = giftcard.customer_id
)
 
SELECT
  first_name,
  last_name,
  payment_date
FROM ranking
WHERE rank = 2;
```
### Calculate Running Total for Payments
For each single rental, show the id, rental_date, payment_amount and the running total of payment_amounts of all rentals from the oldest one (in terms of rental_date) to the current row.

```sql
SELECT
  id,
  rental_date,
  payment_amount,
  SUM(payment_amount) OVER(
    ORDER BY rental_date
    ROWS BETWEEN UNBOUNDED PRECEDING AND CURRENT ROW)
FROM single_rental;
```

First, we select information about each single rental from the single_rental table.

Next, we are going to find the running total of payment amounts of all rentals using the SUM() function (which takes the payment_amount column as its argument) with the OVER() clause. Here is an article explaining the details about running total and how to compute it in SQL.

The instruction says to find the running total from the oldest rental date until the current row date. So, in the OVER() clause, we need to order the data by the rental_date column and then define ROWS to be counted in the running total, from the oldest date (BETWEEN UNBOUNDED PRECEDING) until the current date (AND CURRENT ROW).

## Dataset
- The `doctor` table stores information about doctors. The columns are `id`, `first_name`, `last_name`, and `age`.
- The `procedure` table contains information about procedures performed by doctors on patients. The columns are `id`, `procedure_date`, `doctor_id` (references the doctor table), `patient_id`, `category`, `name`, `price`, and `score`.

### Calculate Moving Average for Scores
For each procedure, show the following information: procedure_date, doctor_id, category, name, score and the average score from the procedures in the same category which are included in the following window frame: the two previous rows, the current row, and the three following rows in terms of the procedure date.



```sql
SELECT
  procedure_date,
  doctor_id,
  category,
  name,
  score,
  AVG(score) OVER(
    PARTITION BY category
    ORDER BY procedure_date
    ROWS BETWEEN 2 PRECEDING AND 3 FOLLOWING)
FROM procedure;
```

### Find the Difference Between Procedure Prices
For each procedure, show the following information: id, procedure_date, name, price, price of the previous procedure (in terms of the id) and the difference between these two values. Name the last two columns previous_price and difference.

```sql
SELECT
  id,
  procedure_date,
  name,
  price,
  LAG(price) OVER(ORDER BY id) AS previous_price,
  price - LAG(price) OVER(ORDER BY id) AS difference
FROM procedure;
```

### Find the Difference Between the Current and Best Prices
For each procedure, show the:

procedure_date
name
price
category
score
Price of the best procedure (in terms of the score) from the same category (column best_procedure).
Difference between this price and the best_procedure (column difference)

```sql
SELECT
  procedure_date,
  name,
  price,
  category,
  score,
  FIRST_VALUE(price) OVER(PARTITION BY category ORDER BY score DESC)
     AS best_procedure,
  price - FIRST_VALUE(price) OVER(PARTITION BY category
     ORDER BY score DESC) AS difference
FROM procedure;
```

We start by selecting information about each procedure from the procedure table.

The next step is to find the price of the best procedure. We use the `FIRST_VALUE()` function, which returns the first value in an ordered partition of a result set. To get the price of the best procedure from the same category, we must partition the dataset by the category column. And to get the price of the best procedure in terms of score, we must order the dataset by the score column in descending order. We alias this expression as best_procedure.

Lastly, we find the difference between price and best_procedure by subtracting the `FIRST_VALUE()` function from the price column.

### Find the Best Doctor per Procedure
Find out which doctor is the best at each procedure. For each procedure, select the procedure name and the first and last name of all doctors who got high scores (higher than or equal to the average score for this procedure). Rank the doctors per procedure in terms of the number of times they performed this procedure. Then, show the best doctors for each procedure, i.e. those having a rank of 1.

```sql
WITH cte AS (
  SELECT
    name,
    first_name,
    last_name,
    COUNT(*) c,
    RANK() OVER(PARTITION BY name ORDER BY count(*) DESC) AS rank
  FROM procedure p
  JOIN doctor d
    ON p.doctor_id = d.id
  WHERE score >= (SELECT avg(score)
                  FROM procedure pl
                  WHERE pl.name = p.name)
  GROUP BY name, first_name, last_name
)
 
SELECT
  name,
  first_name,
  last_name
FROM cte
WHERE rank = 1;
```

First, we select the procedure name and information about doctors, so we join the procedure table with the doctor table on their common column (doctor_id).

We want to select all doctors who got high scores (higher than or equal to the average score for this procedure). To do that, we define the WHERE clause condition for the score column. The score column must store a value equal to or greater than the average score for the current row’s procedure.

Let's rank the doctors per procedure. We'll use the RANK() function with the OVER() clause, where we partition the dataset by the procedure name. Additionally, we must rank in terms of the number of times the doctor performed this procedure. To get the number of times the doctor performed this procedure, we must COUNT(*) while grouping by the procedure name and the first and last name of the doctor (that is, we are grouping by all columns listed in the SELECT statement).

All we’ve done until now is define a Common Table Expression (CTE), which is the inner SELECT statement enclosed by the WITH clause and named cte.


Now we select the relevant columns from this CTE. To get the best doctors for each procedure (those having a rank of 1), we define the WHERE clause with the condition for the rank column.

Why do we need to define a CTE and then query it? Because we cannot use the rank column in the WHERE clause of the inner SELECT. The reason is the order of execution, which is: FROM, JOINs, WHERE, GROUP BY, HAVING, SELECT, DISTINCT, ORDER BY, and LIMIT. The rank column has not been defined when the WHERE clause is executed.


# Links
- [using NULL sqlzoo](https://sqlzoo.net/wiki/Using_Null)
- [self join sql zoo](https://sqlzoo.net/wiki/Self_join)
- [self join youtube](https://www.youtube.com/watch?v=_Q36m72GJRs)
- [full outer join youtube](https://youtu.be/Yh4CrPHVBdE?t=488)
- [leetcode must try](https://leetcode.com/problems/students-and-examinations/description/?envType=study-plan-v2&envId=top-sql-50)
- [leetcode must try](https://leetcode.com/problems/average-selling-price/?envType=study-plan-v2&envId=top-sql-50)
- [leetcode must try](https://leetcode.com/problems/percentage-of-users-attended-a-contest/?envType=study-plan-v2&envId=top-sql-50)
- [exam q1 stack](https://stackoverflow.com/questions/66019044/how-to-find-the-product-with-the-maximum-discount-using-sql-on-hackerrank)
- [exam q2 stack](https://stackoverflow.com/questions/62356006/sql-count-more-than-average-having-vs-where)
- [window func](https://www.youtube.com/watch?v=y1KCM8vbYe4&ab_channel=ColtSteele)
- [CTE](https://www.youtube.com/watch?v=K1WeoKxLZ5o&ab_channel=AlexTheAnalyst)
- [correlated subquery](https://www.youtube.com/watch?v=SM9cDMxAeK4&ab_channel=EdredoforLearners)
- [??](https://stackoverflow.com/questions/78452722/confusion-between-two-sql-queries)
  - [??](https://www.sisense.com/blog/everything-about-group-by/)
- [Running Total](https://stackoverflow.com/questions/30861919/what-is-rows-unbounded-preceding-used-for-in-teradata)
