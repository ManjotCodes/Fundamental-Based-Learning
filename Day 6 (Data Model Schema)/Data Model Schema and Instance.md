# Data model Schema and Instance
The data which is stored in the database at a particular moment of time is called an instance of the database.
The overall design of a database is called schema.

A database schema is the skeleton structure of the database. It represents the logical view of the entire database.

A schema contains schema objects like table, foreign key, primary key, views, columns, data types, stored procedure, etc.

A database schema can be represented by using the visual diagram. That diagram shows the database objects and relationship with each other.

A database schema is designed by the database designers to help programmers whose software will interact with the database. The process of database creation is called data modeling.

A schema diagram can display only some aspects of a schema like the name of record type, data type, and constraints. Other aspects can't be specified through the schema diagram. For example, the given figure neither show the data type of each data item nor the relationship among various files.

In the database, actual data changes quite frequently. For example, in the given figure, the database changes whenever we add a new grade or add a student. The data at a particular moment of time is called the instance of the database.