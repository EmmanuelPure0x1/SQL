
# SQL Syntax

**SP_HELP '<name>'**
- Shows the structure of a table
- Example: SP_HELP sample

** CREATE DATABASE <name> **
- Creates a database with a specified name
- Example: CREATE DATABASE my_db

** CREATE TABLE <name> {column type} **        
- Creates a table with a specified column name and type
- Example: CREATE TABLE sample { name VARCHAR(10) }

** USE <name> **
- Uses specified database for some data manipulation
- Example: USE my_db

** SELECT <object> FROM <name> **
- Selects a specific object / column / row from a specific table
- Example: SELECT * FROM sample

** ALTER TABLE <name> ALTER <column/row> <name> <type> ** 
- Modifies the table's column or row to a different data type
- Example: ALTER TABLE sample ALTER COLUMN name VARCHAR(255)

- INSERT INTO <name> (column_1, column_2) VALUES ('value_1', 'value_2')
Inserts some data into the columns
Example: INSERT INTO sample (name, surname) VALUES ('John', 'Smith')

- UPDATE <name> SET <column> = <new value> WHERE <column> = <existing value>
Updates data in a specific table based on value in a column
Example: UPDATE sample SET name = 'Dev' WHERE name = 'Hubert'

- DELETE FROM <name> WHERE <column> = <value>
Removes a row based on a value in a column
Example: DELETE FROM sample WHERE name = 'Dev'

- DROP <name>
Deletes an entire table
Example: DROP sample

### Specific Cases

If data type is date you need to insert a format of YYYY-MM-DD.
Example: 20200101
Do not allow NULL. Can be used as Alter or Insert or during Create Table
Example: ALTER COLUMN <name> VARCHAR(255) NOT NULL
Set Primary Key. In create table syntax. Identity is used for Auto-Incrementation => IDENTITY(starting value, increment value)
Example: <column> int IDENTITY(1,1) PRIMARY KEY

### Data Types

** VARCHAR: **
- Adaptable to different lengths of charactes. Records MAX Size.

** CHARACTER or CHAR: ** 
- Data must be at a fixed length. Fixed amount of space used.

** INT: **
- Holds a whole number/integer value positive or negative

** DATE or TIME or DATETIME: ** 
- Stores Date, Time or both Date and Time in one variable

** DECIMAL or NUMERIC: **
- Fixed Precision and scale (digits to right of decimal point) numbers

** BINARY: ** 
- Use to store binary data such as an image or file

** FLOAT: **
- Scientific use (very large numbers)

** BIT: **
- Equivalent to binary (0, 1 or NULL)
