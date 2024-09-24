Sources: MySQL documentation


#EngineDocumentation
# Database Engine

Behind the scenes of "Query OK, 1 row affected (0.00 sec)" a db.opt file is  
created by MySQL that holds database options. The above command search  
all db.opt files.
	`$ find . -name db.opt`

MySQL operates in AUTOCOMMIT mode, so commands we issue at the
MySQL prompt are committed and treated as a transaction.

	SHOW ENGINES;
There are nine types of database engines available and by default, tables get created as InnoDB type.
There are pros and cons of using each type. 
InnoDB supports fine-grained locking at the cost of slower performance but
allows multiple users to make modifications to a table at the same time.
On other hand, MyISAM places whole-table locks to handle multiple users
wich is simpler and faster but reduces concurrency.

<hr>


#commands
# *Basic SQL*

#initcommands

	$ mysql -u username -p password (enter after.  password)

Monitoring and selecting  

    SHOW DATABASES;  
  
To explore a particular database:
  
    USE <database_name>;
i.e:
	`USE mysql;`
  
The **USE** statements allow us to let MySQL know the DB we want  
to interact with. 
To examine how the DB was created:  
  
    SHOW CREATE DATABASE mysql;  
  
What tables the MySQL DB holds:  
  
    SHOW TABLES;  
  
Explore the structure of a table:  
  
    DESCRIBE user;  
Show and describe commands looks similar but, describe is a shortcut from show. Show in other hand, can accept "filter" parameters.
  
Use the SHOW statement to display how the table was created:  
  
    SHOW CREATE TABLE servers;  
  
We can display the column info for a table:
  
    SHOW COLUMNS FROM servers;  

<hr>

# Creating a Database  
#createdatabase
-- Query 1  

    CREATE DATABASE MovieIndustry;
  
-- Query 2 when writing scripts that may be invoked repeatedly  

    CREATE DATABASE IF NOT EXISTS MovieIndustry;
  
-- Query 3 to inspect the changes  

    SHOW DATABASES;

-- Query 4  

    DROP DATABASE MovieIndustry;
  
<hr>
  
Creating a Table
  #createtable
Syntax:

    CREATE TABLE tableName(
    
    col1 <dataType> <Restrictions>,

    col2 <dataType> <Restrictions>,

    col3 <dataType> <Restrictions>,

    <Primary Key or Index definitions>);
  

Column syntax:

`columnName columnType [NOT NULL | NULL] [DEFAULT columnValue]`
  
*i.e*  

    CREATE TABLE Actors (
    Id INT AUTO_INCREMENT,
    FirstName VARCHAR(20) NOT NULL,
    SecondName VARCHAR(20) NOT NULL,
    DoB DATE NOT NULL,
    Gender ENUM('Male','Female','Other') NOT NULL,
    MaritalStatus ENUM('Married','Divorced','Single','Unknown') DEFAULT "Unknown",
    PRIMARY KEY (Id));

-- Alternative Query

    CRREATE TABLE IF NOT EXISTS Actors (
    Id INT AUTO_INCREMENT,
    FirstName VARCHAR(20) NOT NULL,
    SecondName VARCHAR(20) NOT NULL,
    DoB DATE NOT NULL,
    Gender ENUM('Male','Female','Other') NOT NULL,
    MaritalStatus ENUM('Married','Divorced','Single','Unknown') DEFAULT "Unknown",
    PRIMARY KEY (Id));  
  
Some restrictions exist when using AUTO_INCREMENT feature: 
   
- Can be only one column marked as AUTO_INCREMENT in a table.  
- The AUTO_INCREMENT column can't have a default value.  
- The AUTO_INCREMENT column must be indexed.  
- AUTO_INCREMENT feature isn't portable to other databases and counter  
    is reset when truncate or drop a table.  
  
  
# Temporary Table
#temptable

    CREATE TEMPORARY TABLE tableName(
    
    col1 <dataType> <Restrictions>,

    col2 <dataType> <Restrictions>,

    col3 <dataType> <Restrictions>,

    <Primary Key or Index definitions>);
  
Say we want to capture only the first names of actors in a table.  
We can create a temporary table and populate it with only the first name.  

    CREATE TEMPORARY TABLE ActorsNames (
    FirstName CHAR(20));
  
If exit the session and we log back into the monitor program, the temporary 
table ActorNames has been deleted.  
Temporary tables can be used to work with intermediate data or results.  
Also complex queries with joins or nested queries can be broken up and  
worked on step-by-step by storing intermediate results in temp tables.

<hr>

Collations & Character Sets
  
The aviable character sets on the server:

    SHOW CHARACTER SET;

List the collations:  
    
    SHOW COLLATION;

Inspect the defaults for our server.

    SHOW VARIABLES LIKE "c%";


<hr>

# Data Types
#datatypes


# Insert Data
#insertdata

	INSERT INTO table (col1, col2, ... coln)  
	VALUES (val1, val2, ... valn);  

 -- Query 1 
	 `INSERT INTO Actors (` 
	 `FirstName, SecondName, DoB, Gender, MaritalStatus, NetworthInMillions)` 
	 `VALUES ("Brad", "Pitt", "1963-12-18", "Male", "Single", 240.00);`
 
-- Query 2 
	`INSERT INTO Actors ( FirstName, SecondName, DoB, Gender, MaritalStatus, NetworthInMillions) VALUES ("Jennifer", "Aniston", "1969-11-02", "Female", "Single", 240.00), ("Angelina", "Jolie", "1975-06-04", "Female", "Single", 100.00), ("Johnny", "Depp", "1963-06-09", "Male", "Single", 200.00);` 

-- Query 3 
	`INSERT INTO Actors VALUES (DEFAULT, "Dream", "Actress", "9999-01-01", "Female", "Single", 000.00);` 

-- Query 4 
	`INSERT INTO Actors VALUES (NULL, "Reclusive", "Actor", "1980-01-01", "Male", "Single", DEFAULT);` 

-- Query 5 
	`INSERT INTO Actors () VALUES ();` 

-- Query 6 
	`INSERT INTO Actors SET DoB="1950-12-12", FirstName="Rajnikanth", SecondName="", Gender="Male", NetWorthInMillions=50, MaritalStatus="Married";`

SET is another form to insert data in the table. Notice that we dont follow the original order of the table, beacuse we are explicit call the column name
and added a value.


<hr>

# Querying Data
#querydata

The SELECT statement retrieve data from tables.
	`SELECT col1, col2, ... coln`
	`FROM table`
	`WHERE <condition>`

-- Query 1  
	`SELECT * from Actors; 
-- Query 2 
	`SELECT <columns> FROM <TableName>`

-- Query 3 
	`SELECT FirstName, SecondName from Actors;` 

-- Query 4 
	`SELECT FirstName, SecondName from Actors WHERE FirstName="Travolta";`

-- Query 5 
	`SELECT FirstName, SecondName from Actors WHERE FirstName="Brad";` 

-- Query 6 
	`SELECT FirstName, SecondName from Actors WHERE NetWorthInMillions > 500;` 

-- Query 7 
	`SELECT FirstName, SecondName from Actors WHERE NetWorthInMillions > 0;`

The SELECT keyword is followed by a comma-separated list of columns
we wish to display.

	SELECT FirstName, SecondName FROM Actors;

There are various operators that can be used in a WHERE clause.


## LIKE Operator
#filteroperators

Like operator works only with string data types and allows us to retrieve
rows based on pattern matching on a particular column.

	SELECT col1, col2, ... coln
	FROM table
	WHERE col3 LIKE "%some-string"






<hr>

# Creating a View
#views

Views are virtual tables that are created as a result of a SELECT query.
They offer a number of advantages such as showing only a subset of
data that is meaningful to users or restricting the number of rows and
columns shown for security reasons.

A view containing columns from multiple tables can simplify queries
from multi-table query to a single table query against a view.
A view can be created from a single table, by joining two tables, or from
another view.

	CREATE [OR REPLACE] VIEW view_name AS
	SELECT col1, col2, ... coln
	FROM table
	WHERE <condition>




<hr>

# Transactions
#transactions

"A transaction symbolizes a unit of work performed within a database
management system against a database, and treated in a coherent and 
reliable way independent of other transactions".
When multiple users are interacting with a database it is possible for the
actions of one user to interleave with another user and bring the data in
an inconsistent state.
Transactions allow you to batch together SQL statements as an indivisible
set that either succeeds or has no effect on the database.

	START TRANSACTION;
	SQL STATEMENTS
	COMMIT;

	START TRANSACTION;
	SQL STATEMENTS
	ROLLBACK;

