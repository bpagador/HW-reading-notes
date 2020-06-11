#### Reading, Research, Discussion

* Instance Methods in Mongoose
    * documents = instances of models 
    * docs have their own built-in instances (like populate())
    * you can also define your own custom doc instance methods (aka a function you assign a method)
    * but be careful, don't declare method with arrow function (=>)

* Static instances 
    * static methods aren't called on instances of the model, but in the model itself 
    * thereby adding utility to the model that might help it create / find / etc. objects 

* Moongoose middleware
    * aka pre and post hooks that take control when asyc funcs are being executed 
    * for mongoose, they are specified at the schema level and are useful for automizing model logic 