## Vocab:
* native client applications = an applicattion that is installed on a user's computer device
* SQL = structure query language, used to communicate with a database


## General
* in web applications:
    * cookies send the same data over and over again, slowing down your browser
    * cookies send unencrypted data
    * cookies limited to 4kb of data  
* in native client applications:
    * you can embed your own database, invent your own file format, etc
* HTML5 storage = the way web pages store key/value pairs locally, within the client web browser
    * based on key value pairs
    * the named key is a string 
    * the data can be any type supported by JS
        * but it will be stored in a string
        * otherwise use parseInt() or parseFloat()
    * calling setItem() with a named key with overwrite previous value 
    * calling getItem() with a non-existent key will return null
    * you can also just use array brackets to call the item:
        * const foo = localStorage.getItem("bar"); is the same as below
        * const food = localStorage[" bar "];
    * removeItem() needs a named key inside parenthesis to delete key and value of that item
        * without anything inside parenthesis, it deletes nothing
* Modernizr is a wesbite where you can detect support for HTML5 storage
* IndexedDB (formerly WebSimpleDB)
    * contains an object store which contains:
        * database with records
            * each record contains set number of fields
            * each field has a specific datatype, which is defined when the database is created
    * you can select a subset of records, then enumerate with with a "cursor"
    * changes to the object store are handlded within "transactions"
    * the object store does not have a structure query language 
