# SQL

### Introduction to SQL

- With SQL, we can do the following:
	- Queery Databse
	- Joins Queries and Subqueries

### SQL Basics

- Columns - (Down)
- Rows - (Across)
- Table - This is a predefined format of rows and columns that define an entity. These are also known as files.
- DBMS - **D**ata**B**se **M**anagement **S**ystem allows a computer to perform database functions such as **storing**, **retrieving**, **adding**, **deleting**, **modifying** data.


### Relational Databases 

- One to One:
	- Each row in Table A is linked to nomore than one row in Table B. (attirubte of the relationship, not table)
- One to Many:
	- Each row can be related to many rows in the relating table.
	- This allows frequently used information to be saved only once in a table and referenced many times in all other tables.
- Many to Many: 
	- One or more rows in a table can be related to 0, 1 or many rows in another table.
	- A 3rd table called a mapping link table is required in order to implement such a relationship. 

### Primary Key

- Used to identify to table.
- Most tables should have a PK.
- Must be unique.
- Value must never change (primary key).
- One primary key per table.
- Primary key must not be NULL.
- **Compound/Composite* Primary key is 2 or more bits of data making the primary meaning both bits must be present when key is called.
primary key.

### Foreign Key
- Foreign key is a primary key in another table or seconday table. Builds the bond oor connection to primary table or other table.
- Foreign key can exist many times over (Not primary).
- You can turn a primary key in one table to be a foreign key in another so as to be able to refer to it later.
- If a FK or a PK is still in use it cant be deleted.

**DML:**

- select, insert, update, delete

**DDL:**

- Create, alter, Drop, Truncate

**DCL:**

- Grant, Revoke

**TCL:**

- Commit, Rollback, Savepoint

### Database Types: 

- Flat-file DB:
-- Not adviseable as this is unsafe
	- Excel
- Relational DB:
-- Linked via Primary and Foreign Keys
	- SQL
	- PostgreSQL
- Big Data DB:
-- Also known as not only SQL-DB ("NoSQL")
	- MongoDB
	- Vertica
