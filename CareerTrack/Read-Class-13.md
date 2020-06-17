#### Mongo Aggregations
* aggregatation pipeline: framework for data aggregation
    * modeled after data processing pipelines (matching, grouping, yada yada)
* this pipeline can be used to transform documents into aggregated results 
    * includes multi stages
    * each stage transforms the document 
    * stages can appear multiple times in pipelines 
        * except: out, merge, and geoNear
        * tons of pipeline expressions: (https://docs.mongodb.com/manual/meta/aggregation-quick-reference/#aggregation-expressions)

#### Aggregations by Example
* start using an aggregation pipeline by calling the *aggregate* function on any collection 
* the aggregate func accepts an array of data transformation
    * db.collection.aggregate([... aggregation steps/expressions ... ])
* to match : { $match: { "prop": value } }
* to group : { $group: "prop": value, "prop": value}}
* operators that sum, min, max, and avg: 
    * $gt - $gte
    * $lt - $lte
    * total
    * $sum