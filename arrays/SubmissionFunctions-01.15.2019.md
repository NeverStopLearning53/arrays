#Exercises
#Questions

###1 Describe/define DRY and why functions exist.
DRY is an acronym for Don't Repeat Yourself. It is a principle in programming that broadly states that every piece of knowledge must have a single representation within a system. What this means is your code should be broken into components with a single responsibility. Functions are blocks of code that complete an action. They are reusable custom code defined by a programmer; being reusable means you can code less and do more! Functions says you from having to enter the same code over and over.

###2 Describe/define the difference between creating a function and calling/executing a function.

Creating a function (or declaring a function) creates the block of code we want to complete an action. Creating (or declaring) the function does not execute the code. We need to call (or invoke) the function. When we invoke a function the code executes. To invoke a function, write the name of the function followed by parentheses.

###3 Describe/define what arguments/parameters are and how they relate to functions.

* Parameters are variables that hold the values we pass into functions and behave like local variables.

* Arguments are the values we pass to a function's parameters when we invoke the function.

###4 Describe/define mutating vs non-mutating functions. 

* Mutating Functions - Alter an existing object or data structure directly.

* Non-mutating Functions - Produce a new object or data structure.

### Using the `shoppingCart` variable, create a function that takes the `shoppingCart` variable and returns the total cost of both items as the `total` variable. `


```javascript
// the variable shoppingCart is an array
// since the elements inside of array can change we want to write a function which will always be able to total up the elements inside the array
var shoppingCart = [20, 15];
// we are declaring a function getTotalCost which will total up the elements inside the shopping cart array
function getTotalCost(prices){
//prices is the input we are going to use in this function / `prices` is a local variable
//in this case `prices` input is going to use the shopping cart arrays elements
  let total = 0;
  for (let i=0; i < prices.length; i++) 
    { 
    total = prices[i] + total;
    }     
  // code above
  return total;
  
}
//using the input shoppingCart variable execute the getTotalCost Function
getTotalCost(shoppingCart);

```