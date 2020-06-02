
## Reading, Research, and Discussion
* Name 3 advantages to Test Driven Development
    * it allows for a clean design the farther you get into the buildout of your projest, making each new feature easier to work with and integrate( the inverse of TDD being adding and adding features only to find a stack of tech debt in testing functionality and it sucks!)
    * creates mantainable code you can return to over time (especially when you'e spending a couple of yeara building a site), not just working code 
    * using TDD to build a project means you end up with a robust/thorough library of tests, which makes things likes refactoring without breaking code and spinning into chaos infinitely easier
* In what case would you need to use beforeEach() or afterEach() in a test suite?
    * both are useful if you have repeating work/functionality for many tests
    * beforeEach() runs a function <strong>before</strong> each of the tests in the file run
        * useful when you want to reset a global state that will be used by many tests
    * afterEach() runs a function <strong>after</strong> each of the tests in the file run
        * useful when you want to run a function that handles whatever temporary state is created by each test
    * sourced from: Jest Documentation (https://jestjs.io/docs/en/api#beforeeachfn-timeout)
* What is one downside of Test Driven Development
    * test suites have the be maintained, the same as the code dependent on them 
* What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
    * according to developers on the internet who, by the way, seem to HATE the claims that ES6 classes make life easier:
        * both ES6 classes and prototype classes accomplish the same thing, but are syntactically different
    * HOWEVER, here's a quote that breaks down the difference in a way I can understand:
        * "The most important difference between class- and prototype-based inheritance is that a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance."
    * sourced from: As a JS Developer, This Is What Keeps Me Up at Night (https://www.toptal.com/javascript/es6-class-chaos-keeps-js-developer-up#:~:text=Prototypes%20vs.,Classes&text=A%20child%20of%20an%20ES6,t%20implemented%20on%20the%20child.)
* Name a use case for a static method
    * whenever you need to call a method on an object without instantiating a class 
* Write an example of a Higher Order function and describe the use case it solves
```
an example we went over with Ryan:

const multiplybyTwo = int = int * 2
const arrayOfInts = [1, 2, 3, 4]

arrayOfInts.map(multiplyByTwo)

// [2, 4, 6, 8]
```
* the use case it solves: maps over the array to effectively apply a function to that array and return a brand new one

## Memorable notes
* KISS -- Keep it Simple Smarty (James Shore)


## Terms:
functional programming
pure function
higher-order function
immutable state
object
object-oriented programming (OOP)
class
prototype
super
inheritance
constructor
instance
context - still a bit confused with this one, but I think context is the intersection of parameter and scope (the official definition on the internet: can be difined as all revelant information that a developer needs to complete a task)
this
Test Driven Development (TDD) - the best tool in the world according to literally every developer!
Jest
Continuous Integration (CI)
unit test