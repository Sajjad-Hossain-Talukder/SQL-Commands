#### Section 08: [ AS ] : Table-Column
  
| Command    | Description |
| ----------- | ----------- |
| AS  | Used to <b> rename a column or table </b> with an  <b> alias (উপনাম) </b> . <br> An alias only exists for the duration of the query.|
| SELECT <b> CustomerName AS Customer</b>,<b> ContactName AS 'Contact Person'</b> <br> FROM Customers;| Renaming Column with single word or Multiple Words|
|SELECT o.OrderID, o.OrderDate, c.CustomerName<br>FROM <b>Customers AS c, Orders AS o</b><br>WHERE ....... ;|Renaming Table|
|SELECT S_Id as 'Student ID' , S_Name as 'Student Name' , <br> <b> CONCAT_WS(' ',S_Address,S_Email,S_Mobile) as 'Contact Details' </b> <br> from student  ;| Combining Column   |


<br> 

<br>

#### Section 09: [ Constrains ] : Table-Column
  
| Command    | Description |
| ----------- | ----------- |
|NOT NULL | Ensures that a column cannot have a NULL value |
|UNIQUE | Ensures that all values in a column are different|
|PRIMARY KEY | A combination of a NOT NULL and UNIQUE. Uniquely identifies each row in a table|
|FOREIGN KEY  |Prevents actions that would destroy links between tables|
|CHECK | Ensures that the values in a column satisfies a specific condition|
|<b>DEFAULT</b> <br>1] <br> CREATE TABLE Persons (<br>    City varchar(255) <b>DEFAULT 'Sandnes'</b><br>);<br><br>  2] <br>ALTER TABLE Persons <br>ALTER City<b> SET DEFAULT 'Sandnes'</b>;<br> <br> 3]<br> ALTER TABLE Persons <br> ALTER City <b> DROP DEFAULT;</b> <br>|Sets a default value for a column if no value is specified <br> 1] SQL DEFAULT on CREATE TABLE <br>2] SQL DEFAULT on ALTER TABLE  <br> 3] DROP a DEFAULT Constraint <br> |
|CREATE INDEX | Used to create and retrieve data from the database very quickly|
