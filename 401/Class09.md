# Introduction to SQL   

**What is SQL?**

SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database.   

**Relational databases**   

relational database represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.   


**SELECT queries**   

query is just a statement which declares what data we are looking for, where to find it in the database, and optionally, how to transform it before it is returned.   

```
ex:
SELECT column, another_column, …
FROM mytable;
```

The result of this query will be a two-dimensional set of rows and columns, effectively a copy of the table, but only with the columns that we requested.   

To recive all data use:   
```
SELECT * 
FROM mytable;
```

**Queries with constraints**   
In order to filter certain results from being returned, we need to use a WHERE clause in the query.   
```
ex:
SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;
```  


**Filtering and sorting Query results**   
SQL provides a convenient way to discard rows that have a duplicate column value by using the DISTINCT keyword.   

```
ex:
SELECT DISTINCT column, another_column, …
FROM mytable
WHERE condition(s);
```


**Ordering results**   

SQL provides a way to sort your results by a given column in ascending or descending order using the ORDER BY clause.    
```
ex:
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC;
```

**Limiting results to a subset**   
The LIMIT will reduce the number of rows to return, and the optional OFFSET will specify where to begin counting the number rows from.   


```
ex:
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC
LIMIT num_limit OFFSET num_offset;
```


**Inserting rows**   
When inserting data into a database, we need to use an INSERT statement, which declares which table to write into, the columns of data that we are filling, and one or more rows of data to insert.   



**Updating rows**   

to update existing data, which can be done using an UPDATE statement.   

**Deleting rows**  
When you need to delete data from a table in the database, you can use a DELETE statement.   

**Creating tables**  
When you have new entities and relationships to store in your database, you can create a new database table using the CREATE TABLE statement.   


**Altering tables**  
SQL provides a way for you to update your corresponding tables and database schemas by using the ALTER TABLE statement to add, remove, or modify columns and table constraints.   

1. Adding columns
2. Removing columns
3. Renaming the table


**Dropping tables**   
you can use the DROP TABLE statement, which differs from the DELETE statement in that it also removes the table schema from the database entirely.    
