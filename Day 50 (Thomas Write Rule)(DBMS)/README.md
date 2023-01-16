# Thomas write Rule


Thomas Write Rule provides the guarantee of serializability order for the protocol. It improves the Basic Timestamp Ordering Algorithm.

The basic Thomas write rules are as follows:


If TS(T) < R_TS(X) then transaction T is aborted and rolled back, and operation is rejected.

If TS(T) < W_TS(X) then don't execute the W_item(X) operation of the transaction and continue processing.

If neither condition 1 nor condition 2 occurs, then allowed to execute the WRITE operation by transaction Ti and set W_TS(X) to TS(T).

Multiple Granularity
Let's start by understanding the meaning of granularity.

Granularity: It is the size of data item allowed to lock.

# Multiple Granularity:

It can be defined as hierarchically breaking up the database into blocks which can be locked.

The Multiple Granularity protocol enhances concurrency and reduces lock overhead.

It maintains the track of what to lock and how to lock.

It makes easy to decide either to lock a data item or to unlock a data item. This type of hierarchy can be graphically represented as a tree.

For example: Consider a tree which has four levels of nodes.


The first level or higher level shows the entire database.

The second level represents a node of type area. The higher level database consists of exactly these areas.

The area consists of children nodes which are known as files. No file can be present in more than one area.

Finally, each file contains child nodes known as records. The file has exactly those records that are its child nodes. No records represent in more than one file.

### Hence, the levels of the tree starting from the top level are as follows:

Database

Area

File

Record
