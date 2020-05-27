## Problem Domain Article
* vocab to look up:
    * waterfall development
    * Agile (with a capital a) projects
* understanding the problem is the mmost critical part of the equation 
* it's easy to fall into the trap of thinking you understand enough of the problem to get started coding

## JS, Chap 3, pg 100 - 105
* in an object, variables become properties 
* " , functions become methods
* example on property notations
    * hotel.name; is the same as hotel [' name '];

## JS, Chap 5, pg 183 - 242
* document object model  = DOM
* application programming interferance = API
* the DOM tree is the website model, aka the html file 
* .getElementBy...
    * Id()
    * TagName()
    * ClassName()
* .querySelector..
    * () = returns only the first of the matching element
    * All() = returns all
* selecting an element from a nodelist uses The item() method and array syntax (aka index)
* nodeValue replaces the value of the node you've attached it to
    * example:
        * let thing = document.getElementById('the-thing');
        * let changingIt = thing.nodeValue;
        * changingIt = changingIt.replace ('another thing');
        * thing.nodeValue = changingIt
* .textContent grabs the content in the indicated tag
* adding elements using DOM manipulation
    * .createElement() = created element, stored in a value
    * .creatTextNode() = provide content for element, stored in a value 
    * .appendChild() = specifies which element you want this node added to 
* .removeChild () takes on parameter, the reference to the element you no longer want 
* beware of cross-site scripting attacks 
    * using several jQuery methods or innerHTML might lead this to happening?
    



