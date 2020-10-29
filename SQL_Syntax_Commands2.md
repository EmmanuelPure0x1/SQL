# SQL, Day 3

## Syntax 

- It is good practice to start query with a FROM and SELECT * 

```
SELECT *
FROM Orders
```

And then fill out what Information you would like to filter in or out.

#### WHERE & BETWEEN & LIKE & AND & OR

- WHERE goes in after FROM

``` 
SELECT *
FROM Orders
WHERE TerritoryID BETWEEN <value> AND <value>
```
- BETWEEN enables us no to have to evaluate values between the specification.

- If BETWEEN was not present and we only had AND with "TerritoryID >= <value> AND TerritoryID <= <value>;"

We would have to re-specify the variable name as above. eg. VAR >= value AND VAR <= value;

```
SELECT ProductID
FROM Products
WHERE UnitPrice < 5;
```
- Query above is self explanatory.
	- FROM the ProductID TABLE, it SELECTS ProductID column WHERE UnitPrice column value is less than 5.
	
```
SELECT * FROM
WHERE ProductName LIKE 'B%' OR ProductName '%S';
```
#### Using AS for new Columns

```
SELECT ProductID as 'New Name'
FROM Products
WHERE UnitPrice < 5;
```

- With the method above it is also possible to create a new column but within the newly created column modify the column values. Check code below.

```
SELECT ProductName, ProductID, ProductName + ',' + ProductName as 'Name_Doubled'
FROM Products
```
- Be sure to make sure the type of the variable is compatible.

- Using 'IN' to locate and get more accurate results

```
SELECT *
FROM Employees
WHERE Country in ('USA')
```

#### Using DISTINCT

```
SELECT DISTINCT Country
FROM Employees
WHERE Country IS NOT NULL
```
Using DISTINCT is used to return only distinct (different) values. Which means it helps with removing specified duplicate information/output.

### Arithmatic Operators

- '+' (works with DATETIME Columns)
- '-' (works with DATETIME Columns)
- /
- % (Modulo)

#### ORDER BY <value> ASC/DSC

```
SELECT *
FROM [Order Details]
ORDER BY OrderID ASC;

SELECT *
FROM [Order Details]
ORDER BY OrderID DESC;
```

- Both snippets above sorts output in an ASCENDING or DESCENDING manner

#### TOP <number>

```
SELECT TOP 2
FROM [Order Details]
ORDER BY OrderID ASC;
```

- Query above selects only first 2 result from output.
