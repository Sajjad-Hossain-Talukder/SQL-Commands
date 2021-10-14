


#### Section 08 : [ UPDATE ] : ROW 
  
| Command    | Description |
| ----------- | ----------- |
|**UPDATE** table_name <br> SET column1 = value1, column2 = value2, ...<br>WHERE condition;|Used to modify the existing records in a table.|
|<b>DELETE</b> FROM table_name <br>WHERE condition;|Used to delete existing Rows in a table.|

<br> 
<br>
#### Section 09 : [ UPDATE ] : ROW 
  
| Command    | Description |
| ----------- | ----------- |
|**UPDATE** table_name <br> SET column1 = value1, column2 = value2, ...<br>WHERE condition;|Used to modify the existing records in a table.|
|<b>DELETE</b> FROM table_name <br>WHERE condition;|Used to delete existing Rows in a table.|

<br> 
<br>
#### Section 10 : [ AS ] : Table-Column
  
| Command    | Description |
| ----------- | ----------- |
| **AS**  | Used to <b> rename a column or table </b> with an  <b> alias (উপনাম) </b> . <br> An alias only exists for the duration of the query.|
| SELECT <b> CustomerName AS Customer</b>,<b> ContactName AS 'Contact Person'</b> <br> FROM Customers;| Renaming Column with single word or Multiple Words|
|SELECT o.OrderID, o.OrderDate, c.CustomerName<br>FROM <b>Customers AS c, Orders AS o</b><br>WHERE ....... ;|Renaming Table|
|SELECT S_Id as 'Student ID' , S_Name as 'Student Name' , <br> <b> CONCAT_WS(' ',S_Address,S_Email,S_Mobile) as 'Contact Details' </b> <br> from student  ;| Combining Column   |
<br> 
<br>



#### Section 11 : [ Functions ] : Table-Column
  
| Command    | Description |
| ----------- | ----------- |
|**UPPER()** <br> SELECT UPPER (column_name ) as New_name <br> From table_name <br><br> SELECT UPPER('string');|Convert the character case. New_name must Be assigned using AS , else It shows Heading with Upper Keyword . |
|**lOWER()** SELECT LOWER (column_name ) as New_name <br> From table_name <br><br> SELECT LOWER('string');|Convert the character case.|
|**CONCAT()** <br> <br>SELECT CONCAT(column_name1, " ",column_name2, " ",column_name," ",....) AS new_name <br>FROM table_name; <br><br>SELECT CONCAT (exp1," ",exp2," ",....) <br> |Adds two or more expressions/columns together.|
|**CONCAT_WS()** <br> SELECT CONCAT_WS(" ",column_name1,column_name2,column_name,....) AS new_name <br>FROM table_name; <br><br>SELECT CONCAT_WS (" ",exp1,exp2,....) <br> |Do as **CONCAT()** . Only difference , you don't have to put individual space after each string.Put separator at the beginning.  |
|**POW()**<br> SELECT POW(value1,value2) | Return value1 is Powered By value2 |
|**GREATEST()** <br> GREATEST(arg1, arg2, arg3, ...)| Returns the greatest one from arg list.|
|**LEAST()** <br> LEAST(arg1, arg2, arg3, ...)| Returns the smallest one from arg list.|
|**LOG()** <br> Selcet LOG(value) ; <br>Selcet LOG2(value) ; <br>Selcet LOG10(value) ; <br> | LOG(value) - Returns natural Logarithms <br> LOG2(value) - Returns 2-based Logarithms <br> LOG10(value) - Returns Common Logarithm |
|**RAND()** - SELECT RAND()  | Generate random value.|
|<b> More Mathematical Functions : </b><br> **TRUNCATE** - TRUNCATE(number, decimals) <br>**ROUND** - ROUND(number, decimals) <br>**FLOOR** - FLOOR(value)  <br> **CEIL** - CEIL(value)  <br>**ABS** - ABS(value) <br>**SQRT** - SQRT(value) <br> **EXP** - EXP(value) <br>**PI** - PI() <br> **DEGREES** - DEGREES(radians_value) <br> **RADIANS** - RADIANS(degrees_value)| **Truncate()** truncates a number to the specified number of decimal places.<br>Example : TRUNCATE(2.343454,4); = 2.3434 <br><br> **ROUND()** DO same as TRUNCATE().Only Difference is, one can omit decimal value in this Function and in this case it returns decimal portion of Given number <br> Use ROUND rather TRUNCATE <br><br>**Floor()** function returns the largest integer value that is smaller than or equal to a number.<br><br> **CEIL()** function returns the smallest integer value that is bigger than or equal to a number. <br><br>**ABS()** returns Absolute value of given value.<br><br>**SQRT()** function returns the square root of a number.<br><br> **EXP()** - Return e raised to the power of given number. <br><br> **PI()** - Return the value of PI <br><br> **DEGREES()** function converts a value in radians to degrees. <br><br>**RADIANS()** function converts a degree value into radians.|
|<b>Trigonometric Functions : </b>*<br> SELECT **SIN(value)**; <br> SELECT **ASIN(value)**; <br> SELECT **COS(value)**; <br> SELECT **ACOS(value)**; <br> SELECT **TAN(value)**; <br> SELECT **ATAN(value)**; <br> |**SIN(value)**- Returns Sine of given number<br> **ASIN(value)**- Returns ARC Sine of given number<br>**COS(value)**- Returns CoSine of given number<br>**ACOS(value)**- Returns ARC COSine of given number<br>**TAN(value)**- Returns Tangent of given number<br>**ATAN(value)**- Returns ARC Tangent of given number<br>|
<br> 
<br>



#### Section 12 : [ Aggregate Functions - Group Functions ] : Table-Column
  
| Command    | Description |
| ----------- | ----------- |
|<b>Aggregate Functions :</b> | They also known as **Group Functions**.Because they operate on sets of rows and generate a result. |
|**AVG()** <br> SELECT AVG(column_name) AS 'Average Value' From table_name ; |Return the average value for the given column.|
|**COUNT()** <br>SELECT COUNT(column_name) AS 'COUNTER'from table_name ;| Returns the number of records returned by a select query.<br>**Note:** NULL values are not counted.|
|**MIN()** <br>SELECT MIN(column_name) AS 'Minimum' from table_name ;| Returns the minimum data from the records.|
|**MAX()** <br>SELECT MAX(column_name) AS 'Maximum' from table_name ;| Returns the maximum data from the records.|
|**SUM()** <br>SELECT SUM(column_name) AS 'Sum' from table_name |returns the total sum of a numeric column|

<br> 
<br>



#### Section 13 : [ Constraints ] : Table-Column
  
| Command    | Description |
| ----------- | ----------- |
|NOT NULL | Ensures that a column cannot have a NULL value |
|UNIQUE | Ensures that all values in a column are different|
|PRIMARY KEY | A combination of a NOT NULL and UNIQUE. Uniquely identifies each row in a table|
|FOREIGN KEY  |Prevents actions that would destroy links between tables|
|<b>CHECK</b> | The CHECK constraint is used to limit the value range that can be placed in a column.<br>If you define a CHECK constraint on a column it will allow only certain values for this column.<br>If you define a CHECK constraint on a table it can limit the values in certain columns based on values in other columns in the row.<br>https://www.w3schools.com/sql/sql_check.asp |
|<b>DEFAULT</b> <br>1] <br> CREATE TABLE Persons (<br>    City varchar(255) <b>DEFAULT 'Sandnes'</b><br>);<br><br>  2] <br>ALTER TABLE Persons <br>ALTER City<b> SET DEFAULT 'Sandnes'</b>;<br> <br> 3]<br> ALTER TABLE Persons <br> ALTER City <b> DROP DEFAULT;</b> <br>|Sets a default value for a column if no value is specified <br> 1] SQL DEFAULT on CREATE TABLE <br>2] SQL DEFAULT on ALTER TABLE  <br> 3] DROP a DEFAULT Constraint <br> |
|CREATE INDEX | Used to create and retrieve data from the database very quickly|


