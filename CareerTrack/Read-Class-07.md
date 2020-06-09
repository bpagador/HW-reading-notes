#### Reading, Research, Discussion

* Express Middleware Explained Video
    * auto-defined routes do something first
        * it will check for certain parameters, including request and response 
    * then pass it along to the next function
        * once that layer is complete then the function will ask a questions and if true
    * (unless there are more layers of auth/functions) after which the event being handled executed 

* Additional notes on Expres Middleware
    * a series of functions that the request route reads before spitting back the response
        * each func holds re, res, and next
    * two type of middleware:
        * application
            * defines errors, chains other routes, transforms objects, parses, runs on every request
        * route
            * asks specific questions, such as authentification, ip address

* Server Testing
    * Avoiding the actual server for testing means exporting your server as a module in a library
        * is that what our app.js is? a library?!
    * Interested to learn how to wrap superagent in a module and use what sounds like nested agent.js files
        * jest.mock() as a tool within the agent.file of your test 
            * (I don't get it...is the agent file an imported library or something?)
        * jest.mock() is smart enough to use __ mocks __ version of agent file, I assume, to test