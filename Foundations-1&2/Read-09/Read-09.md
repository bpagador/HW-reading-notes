## Introduction to Database Normalization

* Database normalization is a process used to organize a database into tables and columns
* By limiting a table to one purpose you reduce the number of duplicate data contained within your database
* There are three normal forms most databases adhere to using:
    * the first is to minimize duplicate data
    * the second is to minimize or avoid data modification issue
    * the third is to simplify queries

## SQL JOINS
* INNER JOIN
    * This query will return all of the records in the left table (table A) that have a matching record in the right table (table B)
* LEFT JOIN
    * This query will return all of the records in the left table (table A) regardless if any of those records have a match in the right table (table B). It will also return any matching records from the right table
* RIGHT JOIN
    * This query will return all of the records in the right table (table B) regardless if any of those records have a match in the left table (table A). It will also return any matching records from the left table.
* OUTER JOIN
    * This Join can also be referred to as a FULL OUTER JOIN or a FULL JOIN. This query will return all of the records from both tables, joining records from the left table (table A) that match records from the right table (table B).
* LEFT JOIN EXCLUDING INNER JOIN
    * This query will return all of the records in the left table (table A) that do not match any records in the right table (table B)
* RIGHT JOIN EXCLUDING INNER JOIN
    * This query will return all of the records in the right table (table B) that do not match any records in the left table (table A)
* OUTER JOIN EXCLUDING INNER JOIN
    * This query will return all of the records in the left table (table A) and all of the records in the right table (table B) that do not match.