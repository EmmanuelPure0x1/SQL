# SQL

### Introduction to SQL

- With SQL, we can do the following:
	- Queery Databse
	- Joins Queries and Subqueries

### Relational Databases 

- One to One:
- One to Many:
- Many to Many: 

### Primary Key

must be unique
value must never change (primary key)
one primary key by table
primary key must not be NULL
Compound/Composite Primary key is 2 or more bits of data making the primary meaning both bits must be present when key is called.
primary key

### Foreign Key
foreign key is a primary key in another table or seconday table. Builds the bond oor connection to primary table or other table.
Foreign key can exist many times over (Not primary)
YOu can trun a primary key in one table to be a foreign key in another so as to be able to refer to it later.
if there is a foreign key you cant delete the primary key

**DML:**

- select
- insert
- update
- delete

**DDL:**

- Create 
- alter
- Drop
-Truncate

**DCL:**

- Grant
-Revoke

**TCL:**

- Commit
- Rollback
- Savepoint

# SQL Syntax

### Commands: 

- CREATE DATABASE <my_db>;
- USE <my_db>
- SP_HELP 

```
CREATE TABLE user_info 
(
    first_name VARCHAR(20), 
    last_name VARCHAR(20), 
    birthdate DATE
)
```
