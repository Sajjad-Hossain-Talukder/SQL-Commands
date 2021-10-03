## MySQL Basics

#### Section 01 : [ SHOW | CREATE | DROP ] : Database


| Command    | Description |
| ----------- | ----------- |
| SHOW DATABASES ;    | List all databases on the sql server.      |
| CREATE DATABASE db_name ;  |  To create a new database.|
|DROP DATABASE db_name ; | To delete the whole database | 
|BACKUP DATABASE; |Ask Sir !!!!! | 

<br>

#### Section 02 : [ SHOW | RENAME | DROP ] : Table

| Command    | Description |
| ----------- | ----------- |
|CREATE TABLE table_name ( <br>  column_name_1 data_type (size) NULL/ NOT NULL , <br> column_name_2 data_type (size) NULL/ NOT NULL ,<br> column_name_3 data_type (size) NULL/ NOT NULL , <br>........................................<br>........................................<br> PRIMARY KEY(column_name/s) ,<br> CONSTRAINT fk_name FOREIGN KEY (Column_Name/s) REFERENCES referenced_table_name(referenced_column_Name/s) ON DELETE CASCADE ON UPDATE CASCADE , <br> .......................... ); |  To Create a Table with Primary key and Foreign Keys .<br> <br><b>NOTE : Each Table can have only one Primary Key which may consists of one or more than one Columns . But a table/relation may have multiple Foreign Key .In Case of , Foreign Key Declaration , referenced Column have to be Primary Key in Referenced Table/Relation.|
|RENAME TABLE old_table_name TO new_table_name; | To rename the existing Table. |
|DROP TABLE table_name; | To drop the table. | 
  
<br>
  

#### Section 03 : [ INSERT INTO ] : Table
  
| Command    | Description |
| ----------- | ----------- |  
|INSERT INTO table_name VALUES (value1,value2,value3,......) , (value1,value2,value3,......) , (value1,value2,value3,......), ..... ; | TO add values for all the columns of the table, do not need to specify the column names in the SQL query. However, make sure the order of the values is in the same order as the columns in the table.|
|INSERT INTO table_name (column1, column2, column3, ...) VALUES (value1,value2,value3,......) , (value1,value2,value3,......) , (value1,value2,value3,......), ..... ; |TO insert Data Only in Specified Columns.|
  <br>
  

#### Section 04 : [ SELECT ] : Table


| Command    | Description |
| ----------- | ----------- |
|SELECT column1, column2, ...<br> FROM table_name ;| Used to select data from a database.The data returned is stored in a result table, called the result-set.|
|SELECT * FROM table_name |To see all the fields available in the table|
|SELECT <b>DISTINCT</b> column_name FROM table_name  | Used to return only distinct (different) values. <br> <b>NOTE : Inside a table, a column often contains many duplicate values; and sometimes you only want to list the different (distinct) values.</b>|
  
  

