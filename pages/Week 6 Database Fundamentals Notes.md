## DDL - Data definition language
	- ### Data Types
		- CHAR(n)
			- Fixed-length string of **n** characters
		- VARCHAR(n)
			- Variable-length string of **n** characters
		- TEXT
			- Unlimited variable-length string
		- INT
			- Integer
	- ### DDL Clauses
		- #### CREATE
			- Creates a new table with a set of columns
				- ```sql
				  CREATE TABLE test_table (
				  	DepartmentID INT PRIMARY KEY,
				  	Name VARCHAR(50),
				  	ManagerID VARCHAR(20),
				  	StartDate DATE);
				  ```
		- #### DROP
			- Deleting a column
				- ```sql
				  DROP COLUMN column_name;
				  ```
		- #### ALTER TABLE
			- Allows the editing of existing tables
				- ```sql
				  ALTER TABLE my_table
				  	ADD last_name VARCHAR(50),
				      	first_name VARCHAR(40);
				  ```
				- ```sql
				  ALTER TABLE my_table
				  	DROP COLUMN last_name;
				  ```
		- #### INSERT
		- #### UPDATE
		- #### DELETE