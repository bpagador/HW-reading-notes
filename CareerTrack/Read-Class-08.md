#### Reading, Research, Discussion

* Populate - a mongoose aggregator
    * populate() is used to replace paths in the document with other documents from other collections, such as as:
        * single document
        * multiple docs
        * plain object
        * multiple plain objs
        * all objs returned from a query
    * ref = tells mongoose which model(/ et al) to use during population
        * valid data type to use as refs:
            * ObjectId (not recommended unless you are awesome at mongoose)
            * Number
            * String
            * Buffer
    * note that populated paths lose their original _id and their value is replace by the mongoose doc return from the db
        * to do this you have to make a separate query before returning the results of your path 
    * checking for population:  
        * schema.populated('the field you are checking') will return truth or undefined
    * depopulation is possible by:
        * schema.depopulate('the field you want to depopulate')
    * populating multiple paths:
        * populate({ key: 'value', anotherKey: 'another value' })
    * query conditions and other options
        ```
        populate({
            path: 'myPath'
            match: {property: { $gte: property_quality }},
            select: 'propertyFromMyPath - _id' (not sure about this syntax, look into it)
        })
        ```
    * Populate virtuals
        * a field that mongoose never persists to the database

* Using the ExpressJS 4.0 Router
    * routing APIs such as: 
        * .use
        * .get
        * .param
        * route
    * middleware and routes will happen in the order that they appear