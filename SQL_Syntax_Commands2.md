# SQL, Day_3

##Syntax 

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

#### Using AS for new Columns

```
SELECT ProductID as 'New Name'
FROM Products
WHERE UnitPrice < 5;
```
