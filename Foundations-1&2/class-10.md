## JS Ch. 10, “Error Handling & Debugging”

* order of execution = the order in which statement are processed
* execution context:
    * global : code in the script but not in the function 
    * function: code within the function 
    * eval : executed like code in an internal function
* vairable scope:
    * global : declared outside the func
    * function : " inside the func 
* error objects;
    * error
    * syntaxError
    * ReferenceError : tried to reference a variable that is not declared / within scope
    * TypeError : an unexpected data type that cannot be coerced 
    * RangeError : numbers not in acceptable range
    * URIError : encodeURI() and decodeURI() used incorrectly
    * EvalError : eval() function used incorrectly

* How to deal with errors:
    1. Debug the script to fix errors
        * look at what the error message tells you (consider relevant script, line number, error type)
        * check how the script is running (use console.log tools)
        * use breakpoints where things are going wrong 
            * DEBUGGER keyword, right in the dev tools "sources" to create a break point
    2. Handle errors gracefully
        * once with breakpoints, do the values you expect to happen, happen?
        * break down/ break out smaller parts of code to test
            * write values or variables into the console 
            * call functions from the console
            * check objects for methods and properties
        * check the number of parameters for a function 
* try, catch, finally : handle exceptions : pg. 481
* all about throw : pg. 482/5