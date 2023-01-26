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

2. Union All

Union All operation is equal to the Union operation. It returns the set without removing duplication and sorting the data.

3. Intersect

It is used to combine two SELECT statements. The Intersect operation returns the common rows from both the SELECT statements.
In the Intersect operation, the number of datatype and columns must be the same.
It has no duplicates and it arranges the data in ascending order by default.

4. Minus

It combines the result of two SELECT statements. Minus operator is used to display the rows which are present in the first query but absent in the second query.
It has no duplicates and data arranged in ascending order by default.

