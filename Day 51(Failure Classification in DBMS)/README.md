# Failure Classification

To find that where the problem has occurred, we generalize a failure into the following categories:

* Transaction failure

* System crash

* Disk failure

## 1. Transaction failure

The transaction failure occurs when it fails to execute or when it reaches a point from where it can't go any further. If a few transaction or process is hurt, then this is called as transaction failure.

Reasons for a transaction failure could be -

* Logical errors: If a transaction cannot complete due to some code error or an internal error condition, then the logical error occurs.
* Syntax error: It occurs where the DBMS itself terminates an active transaction because the database system is not able to execute it. For example, The system aborts an active transaction, in case of deadlock or resource unavailability.

## 2. System Crash

System failure can occur due to power failure or other hardware or software failure. Example: Operating system error.
Fail-stop assumption: In the system crash, non-volatile storage is assumed not to be corrupted.


## 3. Disk Failure

It occurs where hard-disk drives or storage drives used to fail frequently. It was a common problem in the early days of technology evolution.
Disk failure occurs due to the formation of bad sectors, disk head crash, and unreachability to the disk or any other failure, which destroy all or part of disk storage.
