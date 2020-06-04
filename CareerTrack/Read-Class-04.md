#### Reading, Research, Discussion
* NOTE: Questions 1 - 4, and 7 are in Read-Class-03!


5. Describe how NoSQL Databases scale horizontally
    * In order to handle the demands of a large, growing database, NoSQL horizontally scales by adding multiple servers to the database -- each of those servers performing localized, specific, load-sharing roles. 

6. Give one strong argument for and against NoSQL Databases
    * In favor: NoSQL can be the easiest, cheapest, most adaptable way to manage large and constantly evolving data. 
        * Also localized servers can make database distribution way easier and more convenient. 
        * Against: There's always the persky matter of reliability in the data. Considering that NoSQL is not relational and takes in a tremendous amount of "disorganized" ( not really, but kinda ) data, the possibilities for duplicates in instances where these can be damaging (hospitals, banks, authentification in general) is high. 
        * Sourced from Database Scaling : Horizontal and Vertical Scaling (https://hackernoon.com/database-scaling-horizontal-and-vertical-scaling-85edd2fd9944)

8. Name 3 cloud based NoSQL Databases
    * MongoDB
    * Amazon DynamoDB
    * Cloud BigTable (Google Cloud)


#### Terms
* database
* data model
* CRUD - create, read, update, delete
* schema - strict data model
* sanitize - $ 
* Structured Query Language (SQL)
* Non SQL (NoSQL)
* MongoDB - database that doesn't use schemas
* Mongoose - object modeling library
* record
* document - what rows of information are called in MongoDB
* Object Relation Mapping (ORM) - what mongoose does 