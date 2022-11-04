# Three Schema Architecture

1. The three schema architecture is also called ANSI/SPARC architecture or three-level architecture.

2. This framework is used to describe the structure of a specific database system.

3. The three schema architecture is also used to separate the user applications and physical database.

4. The three schema architecture contains three-levels. It breaks the database down into three different categories.


## Objectives of Three schema Architecture
The main objective of three level architecture is to enable multiple users to access the same data with a personalized view while storing the underlying data only once. Thus it separates the user's view from the physical structure of the database. This separation is desirable for the following reasons:


* Different users need different views of the same data.

* The approach in which a particular user needs to see the data may change over time.

* The users of the database should not worry about the physical implementation and internal workings of the database such as data compression and encryption techniques, hashing, optimization of the internal structures etc.

* All users should be able to access the same data according to their requirements.

* DBA should be able to change the conceptual structure of the database without affecting the user's

* Internal structure of the database should be unaffected by changes to physical aspects of the storage.


## Internal Level
DBMS Three schema Architecture

The internal level has an internal schema which describes the physical storage structure of the database.

The internal schema is also known as a physical schema.

It uses the physical data model. It is used to define that how the data will be stored in a block.

The physical level is used to describe complex low-level data structures in detail.

* The internal level is generally is concerned with the following activities:

1. Storage space allocations.
For Example: B-Trees, Hashing etc.

2. Access paths.
For Example: Specification of primary and secondary keys, indexes, pointers and sequencing.

3. Data compression and encryption techniques.

4. Optimization of internal structures.

5. Representation of stored fields.