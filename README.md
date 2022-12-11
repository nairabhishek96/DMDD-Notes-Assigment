<h2><p align="center">DMDD Lecture Notes</p></h2>


1) A Database Transaction is a set of SQL statements that are executed in a sequence. A DB 
Transaction is created when there is a need to change or update records in tables.

2) Each transaction must be completely executed. It may not be a partial failure because that might 
introduce inconsistencies across databases or tables which is not desirable.

3) For example, if some funds are debited from the sender's bank account but the transaction fails 
before the funds are credited to the receiver's bank account, this results in an inconsistent state.

4) We must ensure that the database satisfies the ACID properties.
A means Atomicity - Atomicity prevents updates to the database from occurring only partially, which 
can cause greater problems than rejecting the whole series outright.
C means Consistency - After a successful write, update or delete of a Record, any read request 
immediately receives the latest value of the value to the one that is issuing a read request.
I mean Isolation - one transaction initiated by one request cannot be interfered by a transaction 
initiated by another request.
D means Durability - It will return to the same state which was there before the disaster.

5) We can use the statement SET auto commit = 1 to ensure that all the queries are committed to 
the database automatically.

6) We can use BEGIN statement to show that is the start of the transaction and the END statement 
to show that it is the end of the transaction in MySQL.

7) A View is just like the virtual view that is created by the select statement. We can use this view to 
work on a select list of records that is shown by the view and we can use this view when the VIEW is 
invoked.

8) Below are the uses of VIEW in the database,
a) It restricts data access,
b) hide the complexity of the data
c) store the complex queries

9) In databases, permissions are important in the sense that we can certain users should be provided 
only with minimum permission to ensure there is no security violation. We can use DCL commands
like GRANT and REVOKE for the same. GRANT is basically to provide permission to the database 
users for reading or writing from the database. REVOKE statement is used to remove the 
permissions from the existing database users.

10) For GRANT, we need to specifically specify the permission and for REVOKE, if one user is 
removed, all the permissions provided by that user will also be removed
