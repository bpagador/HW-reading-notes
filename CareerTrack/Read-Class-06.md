#### Readings: HTTP and REST
* HTTP:
    * used to build distributed, collaborative, hypermedia information systems
    * foundation of the www
    * server =  a host designed to provide a service
    * clients = hosts that make requests to that service
    * http defines how requests and responses should be formatted 

* HTTP Requests:
    * think of all the methods you've worked with:
        * GET
        * POST
        * PUT
        * PATCH
        * DELETE
        * ^^ these are requests
    * the definition of HEADERS here is poor, doesn't really answer my question of: what are headers, exactly?
        * found this on SoapUI that sort of makes sense:
            * Headers carry information for:
                * Request and Response Body
                * Request Authorization
                * Response Caching 
                * Response Cookies
            * Headers should not be confused with paramenters which the specify the variable parts of your resource: the data you are working with

* HTTP Response: 
    * contains:
        * HTTP version
        * status code (for example, 200)
        * status message (OK -- the best)

* Swagger/Open API:
    * "live" documentation system
    * the documentation allows you to generate the swagger documentation by visiting your API and analizing the output
        * ( so it lets you make your own API?); copying and pasting instructions on how generate your own swagger documentation:
            * Visit and review the docs and overview at Swagger.io
            * Sign in to the Swagger Inspector
            * Visit your API, using all applicable REST endpoints and data
            * Note that on the right side, it’ll keep your history
            * Once you’ve gone through all of your routes, use the radio buttons select the routes you want to document
            * Click the “Create API Definition” button
            * Follow the instructions to import your new API documentation to Swagger Hub
            * You can leave it running there, or download the definition as .yml or .json and use it in your own project

* What is a RESTful API? Video:
    * good review on API
    * new take-away, @9:47
        * Authentication presented as command lines (preceded by "curl"), but doesn't go into detail about how to see the command itself
        * look into this later today

