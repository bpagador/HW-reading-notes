#### Reading, Research, and Discussion
* Why would a developer choose to make data models?
    * They might be building a site that requires particular products/images/preferences be directly linked to a specific user. In order to do this, data models organize the input data (or data in general) of the user and make it easier for the developer to distribute the information across the site/multiple schemas.

* What purpose do CRUD operations serve?
    * C = create
    * R = read
    * U = update
    * D = delete
    * these are four basic functions all data models should be able to do 
    * source: What is CRUD? (https://www.codecademy.com/articles/what-is-crud)

* What kind of database is Postgres? What kind of database is MongoDB? 
    * Postgres communicates with SQL, which is relational data structuring and depends on a universal schema set for every piece in the data model. There is no schema in MongoDB's data structure, meaning you have different looking "documents" (rows in a table) in a "collection" (the table). 

* What is Mongoose and why do we need it?
    * Mongoose is an Object Data Modeling library, meaning that it helps organize data models based on the objects, not the schemas, of a database. Mongoose helps with the abstraction created by a no-schema database like MongoDB, making it easier for the developer to implement validation and features tracking CRUD performance in MongoDB.
    * source: Stack Overflow (https://stackoverflow.com/questions/18531696/why-do-we-need-what-advantages-to-use-mongoose) 

* Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department
    * Patients - tracks incoming patients to a hospital
    * Tested for COVID - they are tested for COVID immediately, this piece of data would answer the query with True or False
    * Results - the results could be either positive (True) or negative (False)
    * Status - depending on these results the patient's status would be updated from a series of options such as:
        * at-home care
        * in-hospital care
        * intensive care
        * recovering
        * ready to be discharge
        * etc.
    * Test again: if the patient's status was hospital-bound and should they reach the "ready to discharge" status, they could then be tested once again, for COVID and for anti-bodies, the results for COVID could either be positive (True) or negative (False)
        * False would lead to the patient being discharged
        * True would lead to the patient's data/process/status be tracked once again, starting at Results
    * The contraints have mostly to do with how linear, data-tree like, the tracking information for each patient is. Each data piece following Patients info is reliant on the following data piece. 

#### General Notes:
* sql vs mongo db is a thing I guess!

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