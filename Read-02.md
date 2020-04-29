## Thinking in React
* single responsibility principle: break things down into small pieces 
* UI and data models tend to adhere to the same info architecture
* a good practice is:
    1. identify the components, define what they do
    2. arrange the into a hierarchy, like an essay outline 

## UI Components by Design
* two type of components:
    * Foundation Components are the primary expression of the design language of the system. They’re the defining parts of the experience, and very targeted in scope. They ensure a consistent underlying interface. UI Developers on the design team will build them.
    * Application Components are specific to one of the applications being built, and not seen as a defining, foundational part of the UI. They’re usually larger in scope, and almost always composed of one or many Foundation Components. Some Application Components may eventually transition into Foundation Components. The application teams will build them.
* component centric flow:
    * learn
    * design
    * isolate
    * elaborate
    * build
    * integrate
    * this is a circle that repeats itself 

# Callbacks
* what is a callback:
    * simply put: A callback is a function that is to be executed after another function (normally asynchronous) has finished executing — hence the name ‘call back’.
    * more complexly put: In JavaScript, functions are objects. Because of this, functions can take functions as arguments, and can be returned by other functions. Functions that do this are called higher-order functions. Any function that is passed as an argument and subsequently called by the function that receives it, is called a callback function.

# Classes
* example:

```
class User {
  constructor(name) { this.name = name; }
  sayHi() { alert(this.name); }
}

// proof: User is a function
alert(typeof User); // function
```
* what class User {...} construct really does is:
    * creates a function named User, that becomes the result of the class declaration. the function code is taken from the constructor method (assumed empty if we don’t write such method).
    * stores class methods, such as sayHi, in User.prototype.
* after new User object is created, when we call its method, it’s taken from the prototype. so the object has access to class methods.
