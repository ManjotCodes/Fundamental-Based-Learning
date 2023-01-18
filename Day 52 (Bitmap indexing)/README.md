# Bitmap Indexing

It is a special type of indexing built on a single key. But, it is designed to fire queries on multiple keys quickly. We need to arrange the records in sequential order before applying bitmap indexing on it. It makes it simple to fetch a particular record from the block. Also, it becomes easy to allocate them in the block of a file.


## Bitmap Index Structure

The word 'bitmap' comprises of 'bit' and 'map'. A bit is the smallest unit of data in a computer system. A map means organizing things. Thus, a bitmap is simply mapping of bits in the form of an array. In a relation, each attribute carries one bitmap for its value. A bitmap has sufficient bits for numbering each record in the block.

For example, consider a relation Student_record where we wish to find out the female and male students whose score in English is greater than 40. The bitmaps for gender are given in the below image.

## Bitmap Indexing

If the value of a record iis set to Mr, it means the ithbit of the bitmap will be set to 1. Remaining all other bits for Mr in the bitmap will be set to 0. Similarly, the same step proceeds in the case of female students. If for a particular j record, the value is set to Ms, it means the jth bit in the bitmap will be set to 1. All other bits for Ms will be set to 0. Now, if a user wishes to retrieve either a single or all records for female students or male students, i.e., value as Mr or Ms, only need to read all the records of the relation. After reading, select the required records either for Mr or Ms.

However, the bitmap indexing does not allow to select the records quickly. But, it enables the users to read and choose only the required records. As seen in the above example that the user only selected the required records either for female students or for male students.

## Uses of Bitmap Indexing

Including one from the above example, there are following uses of Bitmap indexing:

It enables the user to read and select only the required records or data from a relation.
It is useful for making selections on multiple keys.

Bitmap indexing helps in counting the number of records falling under the selection requirement. It means it makes it easy to count those tuples which are under the selection criteria of the user.

Bitmap indexing is useful as well as necessary in performing queries for data analysis.
The size of a single bitmap is smaller than 1 percent. Thus, its size is smaller than a relation. For example, a record in a relation is of 100 Bytes, and the relation occupies 1% of memory space. Consequently, a single bitmap occupies 1/8th of the space occupied by the relation.

### Deletion and Insertion of Records

Deleting a record from the relation disturbs the sequence of records. The record which gets deleted creates space or gaps in between other records.
Filling such gaps is possible by shifting other records, but it is an expensive task.
Existence bitmap is a solution to this problem. By storing an existence bitmap, we can recognize the deleted records.
In existence bitmap, if a record does not exist, its bit value will be 0-otherwise 1.
Insertion of records is cost-effective. It is because the insertion of a record does not affect the sequence of other records.
Either by merely replacing the deleted records or by appending records to the EOF (end of file), a user can proceed to insert the records.
