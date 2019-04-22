# T-SQL Homework 10

## Chapter 10 Transactions and Concurrency

### Name: Malachi Evans

#### Date: March 20, 2019

-------------

1. What is the purpose of transactions? Why do we use transactions in SQL scripts?
    + to make a single unit of work that queries and modifies data. To makes changes all at one time.
2. Briefly describe each of the ACID properties.
    + Atomic - Either all changes take place, or none do. It is indivisible. 
    + Consistency- The state of the transaction must remain consistent.
    + Isolation - If a current state is being used you can’t use it elsewhere.
    + Durability - The data is kept in a transaction log. / It’s a permanent change. 
3. What do we mean when we talk about the granularity of locks?
    + The level the lock is on. 
4. What do we mean when we talk about the modes of locks?
    + whether its exclusive locked or shared. Exclusive locked to one user. shared can be used by another user until released.
5. In your own words, describe blocking, and give an example.
    + if we request the same data resource but with different lock types on request will be blocked and will wait until released.
6. What are the properties of locks? That is, list the column name and column type of the fields in
sys.dm tran locks.
+ https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-tran-locks-transact-sql?view=sql-server-2017
7. What are the properties of sessions? That is, list the column name and column type of the fields in
sys.dm exec connections.
+ https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-exec-connections-transact-sql?view=sql-server-2017
8. What are the requests of sessions? That is, list the column name and column type of the fields in
sys.dm exec requests.
+ https://docs.microsoft.com/en-us/sql/relational-databases/system-dynamic-management-views/sys-dm-exec-requests-transact-sql?view=sql-server-2017
9. What is an isolation level? Give an example of the operation of an isolation level.
    + Isolation levels determine the level of consistency you get when you interact with data. 
10. (Not in the book.) What do we mean when we say that an object is serializable?
    + It can be cataloged 
11. What is a deadlock? Give an example of a deadlock?
    + When two tranactions cancel each other.
