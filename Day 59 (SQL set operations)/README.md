# SQL Set Operation

The SQL Set operation is used to combine the two or more SQL SELECT statements.

## Types of Set Operation

Union

UnionAll

Intersect

Minus

## DBMS SQL Set Operation

1. Union
The SQL Union operation is used to combine the result of two or more SQL SELECT queries.
In the union operation, all the number of datatype and columns must be same in both the tables on which UNION operation is being applied.
The union operation eliminates the duplicate rows from its resultset.

Syntax


SELECT column_name FROM table1  

UNION  

SELECT column_name FROM table2;  
