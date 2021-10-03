## MySQL Basics

#### Section 01 : [ SHOW | CREATE | DROP ] : Database


| Command    | Description |
| ----------- | ----------- |
| SHOW DATABASES ;    | List all databases on the sql server.      |
| CREATE DATABASE db_name ;  |  To create a new database.|
|DROP DATABASE db_name ; | To delete the whole database | 
|BACKUP DATABASE |Ask Sir !!!!! | 


#### Section 02 : [ SHOW | RENAME | DROP ] : Table

| Command    | Description |
| ----------- | ----------- |
|CREATE TABLE table_name ( <br>  column_name_1 data_type (size) NULL/ NOT NULL , <br> column_name_2 data_type (size) NULL/ NOT NULL ,<br> column_name_3 data_type (size) NULL/ NOT NULL , <br>........................................<br>........................................<br> PRIMARY KEY(column_name/s) ,<br> CONSTRAINT fk_name FOREIGN KEY (Column_Name/s) REFERENCES referenced_table_name(referenced_column_Name/s) ON DELETE CASCADE ON UPDATE CASCADE , <br> .......................... ); |  To Create a Table with Primary key and Foreign Keys .<br> <br><b>NOTE : Each Table can have only one Primary Key which may consists of one or more than one Columns . But a table/relation may have multiple Foreign Key .In Case of , Foreign Key Declaration , referenced Column have to be Primary Key in Referenced Table/Relation.|
|RENAME TABLE old_table_name TO new_table_name | To rename the existing Table |
