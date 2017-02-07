CLOSURE

What is closure?

Closure is a function inside other function that has access to the variables of the function outside, even after its has returned.
For example, consider this simple code:


function User(name) {

  this.say = function(phrase) { 
    alert(name + ' says: ' + phrase)
  }
}
 
var user = new User('John')


It means that the closure of this code is:

  this.say = function(phrase) { 
    alert(name + ' says: ' + phrase)
  }

The closure has access to three things:
1. its own variables
2. the outer function's variables
3. the global variables


Where is it used?

Closure is commonly seem in Node.js, also jQuery and all the javascripts' code.




References:
1. http://www.w3schools.com/js/js_function_closures.asp
2. https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures
3. http://javascriptissexy.com/understand-javascript-closures-with-ease/