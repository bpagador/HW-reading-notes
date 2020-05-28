## Readings: Node Ecosystem, TDD, CI/CD
* Why would you want to run JavaScript code outside of a browser?
    * As far I understand, using JS outside of a browser is effectively using node.js technology to work with that code. That considered, you likely want to use JS outside of a browser so you can manipulate it, modify it, add functionality using packages, etc.
        * Used Quora to understand "using javascript in browser" because I definitely don't know that means. (source = https://www.quora.com/What-exactly-does-running-JavaScript-inside-a-browser-and-outside-of-a-browser-mean) 
* What is the difference between a module and a package? 
    * The terminology here is interchangeable. Whether you call it package or module, these modular pieces of code accomplish that same thing: solve a (small) problem and solve it well, so that teams can build larger, custom programs from them. 
* What does the node package manager do? 
    * A few different things but mainly NPM holds a bunch of downloadable packages in the NPM site. Also in the NPM client, users can save the code they want to share to the NPM registry so that other users can grab that code and apply it to their own work, create a different version, etc. 
* Provide code snippets showing 3 different ways to export a function from a node module

    ```
    example 1:

    module.exports = {
        nodeFunction
    }
    
    example 2: 

    module.exports = nodeFunction {
        this.key = 'value';
    }

    example 3:

    module.exports = nodeFunction(random) {
        console.log(random);
    }

    ```

## Vocabulary
* ecosystem
* Node.js - an open source server environment of endless possibilities (it can create, open, read, write, deleter, abd close files in the server, collect form data, add, delete, modify data in your db)
* V8 Engine - chrome engine that translates javascript into machine code
* module
* package - a directory with one or more files in it 
* node package manager (npm)
* server
* environment
* interpreter - denotes a node.js installation on a remote host/ virtual environment
* compiler - V8 is a compiler for example, it compiles computer language to machine code 

sources for definitions, "export function from a node module" research, general learning:
* https://www.w3schools.com/nodejs/nodejs_intro.asp
* https://www.tutorialsteacher.com/nodejs/nodejs-module-exports
* https://stackify.com/node-js-module-exports/