## MDN URLSearchParams built-in class (Links to an external site.)
* URLSearchParams interface defines utility methods to work with the query string of a URL
* URLSearchParams
    * .append()
    * .delete()
    * .entries()
    * .forEach()
    * .get()
    * .getAll()
    * .has()
    * .keys()
    * .set()
    * .sort()
    * .toString()
    * .values()

## Built-in Location Object (Links to an external site.)
* properties of Location
    * .ancestorOrigins
    * .href
    * .protocol
    * .host
    * .hostname
    * .port
    * .pathname
    * .search
    * .hash
    * .origin

## Hash change event
```
window.addEventListener('hashchange', function() {
  console.log('The hash has changed!')
}, false);
```
* example ^

## Regex
* Regular expressions (regex or regexp) 
* extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern (i.e. a specific sequence of ASCII or unicode characters)
* you can actually use this tool in (almost) all programming languages ​​(JavaScript, Java, VB, C #, C / C++, Python, Perl, Ruby, Delphi, R, Tcl, and many others)
* flags:
    * g (global) does not return after the first match, restarting the subsequent searches from the end of the previous match
    * m (multi-line) when enabled ^ and $ will match the start and end of a line, instead of the whole string
    * i (insensitive) makes the whole expression case-insensitive (for instance /aBc/i would match AbC)
* look-ahead and Look-behind
    * (?=) and (?<=)
* back-references 
    * \1
* boundaries 
    * \b and \B

## JavaScript Asynchronous Programming and Callbacks
* asynchronous means that things can happen independently of the main program flow
* javaScript is synchronous by default and is single threaded -- this means that code cannot create new threads and run in parallel
* you can’t know when a user is going to click a button, so what you do is, you define an event handler for the click event
    * this is the so-called callback
* the problem with callbacks
    * every callback adds a level of nesting, and when you have lots of callbacks, the code starts to be complicated very quickly
* alternatives to callbacks
    * promises
    * async/await

## Javascript Promises
```
let done = true

const isItDoneYet = new Promise((resolve, reject) => {
  if (done) {
    const workDone = 'Here is the thing I built'
    resolve(workDone)
  } else {
    const why = 'Still working on something else'
    reject(why)
  }
})
```
* the promise checks the done global variable, and if that’s true, we return a resolved promise, otherwise a rejected promise
* using resolve and reject we can communicate back a value, in the above case we just return a string, but it could be an object as well

## Fetch
1. fetch() makes network request to a url and returns a promise.
2. That promise resolves with a response object when the remote server responds with headers.
3. To read the response body, we have to call a response method on it, like text() or json(), which will return another promise whose resolve value is the body of the response.

```
fetch(‘https://jsonplaceholder.typicode.com/users/1')
  .then(function(response) {
    return response.json()
  })
  .then(function(myJson) {
   console.log(myJson);
  });
```
* fetch isn't just for getting
    * simply pass in an object to fetch() that specifies the type of request you want to make, along with the headers and body and whatever else you need
    ```
    fetch(url, {
    method: 'post',
    headers: {
      "Content-type": "application/json; charset=UTF-8"
    },
    body: 'foo=bar&lorem=ipsum'
  })
  .then(json)
  .then(function (data) {
    console.log('Request succeeded with JSON response', data);
  })
  .catch(function (error) {
    console.log('Request failed', error);
  });
    ```
