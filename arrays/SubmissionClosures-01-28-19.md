# **Exercises**
# **Questions**

##### **1 What does "lexical scope" mean in JavaScript?**

A convention used within programming languages that sets the scope of a variable so that it can only be referenced from within the block of code in which it is defined.

##### **2 What is an advantage of a programming language that uses lexical scoping?**
It allows us to reuse variables since they can be defined locally versus globally.
It allows us to use less memory by using local variables versus global variables.
It allows global variables declared outside functions to be used inside functions.


##### **3 What is a closure?**

Closures are nothing but functions with preserved data.
A closure is a function having access to the parent scope, even after the parent function has closed.

##### **4 What would be a use case of a closure?**

In this example we have a problem ...

```
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Closures</h2>

<p>Counting with a local variable.</p>

<button type="button" onclick="myFunction()">Count!</button>

<p id="demo">0</p>

<script>
// Function to increment counter
function add() {
  var counter = 0;
  counter += 1;
  return counter;
}
// Trying to increment the counter
function myFunction(){
  document.getElementById("demo").innerHTML = add();
}
</script>

</body>
</html>
```


We want the count to increase by one each time the count button is pressed but each time the variable counter is being reset to 0 so we can't go above 1 even though we press the count button multiple times.
It did not work because we reset the local counter every time we call the function.
Here is the solution:

```
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Closures</h2>

<p>Counting with a local variable.</p>

<button type="button" onclick="myFunction()">Count!</button>

<p id="demo">0</p>

<script>
var add = (function () {
  var counter = 0;
  return function () {counter += 1; return counter;}
})();

function myFunction(){
  document.getElementById("demo").innerHTML = add();
}
</script>

</body>
</html>
```

The variable add is assigned the return value of a self-invoking function.
The self invoking function only runs once. It sets the counter to zero (0), and returns a function expression.
This way add becomes a function. The "wonderful" part is that it can access the counter in the parent scope.
The solution is to use a JavaScript **closure.** It makes it possible for a function to have **"private"** variables.
The counter is protected by the scope of the anonymous function, and can only be changed using the `add` function.