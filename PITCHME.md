## NodeJs
---
### Functions:
##### 1) Function statement:
```
function calcRectArea(width, height) {
  
	return width * height;

}
 console.log(calcRectArea(5, 6));
```
---
##### 2) Function expression:
```
var getRectArea = function(width, height) {

    return width * height;

}
 console.log(getRectArea(3,4));

// expected output: 12
```
---
##### 2. a) Anonymous methods
var myFunction = function() {
    statements
}
---
##### Named function expression
```
var myFunction = function namedFunction(){
    statements
}
```
Benefit of named function expression is that in case we encountered an error, 
the stack trace will contain the name of the function, making it easier to find the origin of the error.
---
##### 2. b) IIFE
```
var counter = 0;
var f = function(){
	counter++;
	console.log(counter);
}
f();
counter++;
f();
```
---
```
var counter = 0;
var f = function(){
	var counter = 5;
	console.log(counter);
}
f();
counter++;
f();
```
---
```
var counter = 0;
(function(){
	var counter = 5;
	console.log(counter);
})();
counter++;
console.log(counter);
```
---
##### Pros of IIFE:
a) Improving performance, since javascript first looks upto local scope
b) Simulatting or creating a new scope
c) Avoding scope pollution
d) Called once, can also be used to initialize variables
---

##### Arrow functions:
```
([param[, param]]) => {
   statements
}
```

```
param => expression
```

---
IO operations

read file, DB calls,
In C#, Java multi threaded app
In nodejs single threaded event loop

callback
events

---
