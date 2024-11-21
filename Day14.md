# SQL 
Introduction to Databases
 - Why Databases?
       - Alternatives: CSV file,text file,excel file are all flat files.
       - Data base makes our life simpler,easier,faster,relatableand secure.
       - Eg: Finding rows where values of a particular column>10 is time consuming in flat files.Databases use a technique called indexing with simple and easy to uselanguage called SQL to achieve the result faster.
       -Database breaks up the data to different places to increase reliability.
       -Example: Oracle,MySQL,SQL,server.
   - DB contains one or more tables mainly.

## Relational and Non Relational Databases
 - Relational : (Traditional DB(from 1970) like the one listed above):A relational DB
- Stores data in tables
  
## Tables 
   - In a relational databse all of our data is stored across multiple tables
   - movie_id,movie_name,year,actor_id,actor_name,gender
          1            Spiderman
          1            Spiderman,2009,aid_2,name,male
   - Here only some part of data changes other part we are simply copying which is inefficient.
   - In relational databases data is stored across multiple tables to avoid data duplication
                - Table 1: movie_id,movie_name,year
                - Table 2:


  - There is a Primary key associated with each tables.

Why SQL
    - SQL stands for Structured Query Language
       - has its beginings from 1970s

- SQL is not a general purpose programming language,it is domain specific language.
- General purpose programming language lets you create web/mobile apps,games,DBs,Operating systems etc.
- C/C++,Python,etc


Execution of an SQL statement
   - The execution follows the following actions
   - SQL->Parser,Compiler
        ->parser:tries to understand the query
        ->compiler: query optimizer(optimal way to execute) and general code.

## IMDB Database



# Keywords
 - SELECT
 - DISTINCT
 - FROM
 - WHERE
 - LIMIT
 - OFFSET
 - ORDER BY

### SELECT * FROM world; - displays full table
### SELECT * FROM world LIMIT 2; - displays 2 rows
### SELECT name FROM world; - displays name of countries
### SELECT population FROM world
      WHERE name = 'France'
### SELECT name,population FROM world; - displays name and population 
### SELECT * FROM world ORDER BY population DESC; - displays population in descending order
### SELECT * FROM world ORDER BY population DESC LIMIT 8; - displays population in descending order upto 8 countries.
### SELECT DISTINCT continent FROM world; - displays continents
### SELECT name,continent,gdp FROM world WHERE continent<>"Asia"; - continent Asia is excluded.
### SELECT name,continent,gdp
FROM world
WHERE gdp IS NULL; - displays name,continent where gdp is null.
### Logical Operators 
     - And,OR,NOT,ALL,ANY,BETWEEN,EXIST,IN,LIKE,SOME

### SELECT * 
FROM world 
WHERE NOT population<200000;
### SELECT name.population FROM world
  WHERE name IN('Brazil','Russia','India','China');
### SELECT name AS country_name
 FROM world
 ### SELECT name,population,area FROM world 
WHERE area > 3000000 XOR population > 250000000; - displays countries that have population greater than 250 million or area greater than 3 million ,but not both.
  



## Aggregate functions 
- count
- min
- max
- average
- sum
  
## Group By
- often used with count , min,max or sum
-  if grouping columns contains null value, all null values are grouped together
## Having 

order of execution
- group by
- apply aggregate conditions
- apply Having condition

  
 ### Select * from where G-H-O-L
- G : group by
- H : Having
- O : Order by
- L : Limit (has offset)

  ## JOIN
  - INNER JOIN :COMMON IN BOTH TABLES
  - LEFT JOIN : left table + common in tableB
  - RIGHT JOIN : common in table A + tableB
  - FULL OUTER JOIN : tableA+tableB
  - NATURAL JOIN : same as inner join 
    
  - INNER JOIN
     - select tableA.id,tableA.name,tableB.course
       from tableA
       inner join tableB
       on tableA.id = tableB.id
       NB : use alias for table names to shorten the query
       
    - LEFT JOIN
     - select A.id,A.name,B.course
       from tableA A
       left join tableB B
       on A.id = B.id
       
 - RIGHT JOIN
     - select A.id,A.name,B.course
       from tableA A
       right join tableB B
       on A.id = B.id
       
  - FULL OUTER JOIN
     -select A.id,A.name,B.course
       from tableA A
       right join tableB B
       on A.id = B.id
    
    - NATURAL JOIN
        - select *
          from tableA
          natural join tableB;

    ## NESTED QUERIES
    first inner query is executed then outer query
    IN, NOT IN, EXISTS,NOT EXISTS,ANY , ALL,COMPARISON OPERATORS

    ### CREATE,READ,UPDATE,DELETE
   - CREATE
     -  CREATE TABLE table_name(
         col1 col1_dtype,
         col2 col2_dtype,
        );
        
   - INSERT
       - INSERT INTO students ('id','name') VALUES('1','RAM')
   - UPDATE:
   - ALTER :
      - ALTER TABLE table_name
        ADD column_name datatype;
   - DELETE
   - DROP : 
      -DROP TABLE table_name;
   - TRUNCATE
    
