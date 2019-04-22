# T-SQL Homework 11

## Chapter 11 

### Name: Malachi Evans

#### Date: March 28, 2019

--------------------------

1. Why do we use variables in T-SQL? HOw do you declare and initialize T-SQL variables?
    + You use variables to temporarily store data values for later use in the same batch in which they were declared. use Declare to initialize and set to assign value. DECLARE @i AS INT; SET @i = 10; or DECLARE @i AS INT = 10;
2. Describe what is meant by a batch ﬁle in T-SQL? What is the difference between batches and transactions?
    + batch is one T-SQL statement or more sent to Microsoft SQL Server by the client for execution as a single unit. A transaction is a single statement from start to end. 
3. What is the scope of variables with respect to T-SQL batches?
    + it is local to a defined batch.
4. Write a T-SQL code snippet that returns a data element stating whether the current person can legally purchase alcohol, that is, has reached his 21st birthday.
    + SELECT personname as Name, birthday as Bday FROM PersonData WHERE birthday < '1998-03-28' ;
5. (Not in book) Does T-SQL have a FOR loop construction?
    + no but it can be simulated using while loop.
6. What is a cursor? What is the difference between a relation and a cursor?
    + a nonrelational result with order guaranteed among rows. 
7. How do you declare a temporary table? Why would you declare a temporary table?
    + using the create table syntax but using a pound sign. if you dont have permissions to create a new one.
8. What is the difference between a stored procedure, a user defined function, and a trigger?
    + stored procedure can return sets and can make database and schema changes. user defined cant make any schema or database changes they just return scalar values. a trigger is tied to an event and cant be used with out one. 
9. Write a user defined function that returns a Booleans as to whether a customer may purchase alcohol as of the instant that the function runs.
    + DROP PROC IF EXISTS DrinkingAGE @personname as NVARCHAR, @Bday as DATE = '1998-03-28' RETRUN SELECT personname as Name, birthday as Bday FROM PersonData WHERE birthday < @Bday ;
10. Write a trigger that places a customer in the OFF LIMITS table if he attempt to purchase alcohol when he is underage.
    + CREATE TRIGGER insert_Underage ON dbo.T1 AFTER INSERT
        AS
        SET NOCOUNT ON;

        INSERT INTO dbo.T1_Audit(username, birthday)
        SELECT name, birthday FROM inserted;
        GO
11. Write a stored procedure that deletes customers from the OFF LIMITS table when they have reached their 21st birthday.
    + 
