# Exploratory Queries

## Simple Exploration Queries

### SELECT LIMIT

The simplest exploratory query is your humble servant the SELECT query with a limit.
While most database tools have table viewing features that allow you to achieve the same functionality without a query it's nice to know you can still handle it should that feature not be able to be used. 

Use Case(s):
    - Used when retrieving small sample of tables, potentially writing proof-of-concept(poc) queries that can be pieced together for more complex queries down the line. 
Query Category: 
    - DQL

```
SELECT column1, column2
FROM table
LIMIT 5;
```


### SELECT LIMIT FILTERING      

While the SELECT LIMIT is great to just get an idea of what the data that exists in the table is, you'll more often than not be dealing with more complex problem. For such SELECT LIMIT and some form of Filtering functions will be your bread and butter. 

Use Case(s):
    - Used when building basic structures for more complex queries such as joins
    - Used to get data with constraints

```
SELECT column1, column2
FROM table
WHERE column1 NOT NULL;
```