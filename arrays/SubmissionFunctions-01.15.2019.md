I was able to get my javascript code to work but I am still a little bit confused about using return. I couldn't tell if total was correct until I used console.log(total). I also don't understand the function getTotalCost(prices). Is this a different function than getTotalCost(shoppingCart)? Sometimes I think talking to someone would really help but I guess I will wait for my weekly meeting unless you have another idea.

#Exercises
#Questions

###1 Describe/define DRY and why functions exist.
DRY is an acronym for Don't Repeat Yourself. It is a principle in programming that broadly states that every piece of knowledge must have a single representation within a system. What this means is your code should be broken into components with a single responsibility. Functions are blocks of code that complete an action. They are reusable custom code defined by a programmer; being reusable means you can code less and do more! Functions says you from having to enter the same code over and over.

###2 Describe/define the difference between creating a function and calling/executing a function.

Creating a function (or declaring a function) creates the block of code we want to complete an action. Creating (or declaring) the function does not execute the code. We need to call (or invoke) the function. To invoke a function, write the name of the function followed by parentheses.

###3 Describe/define what arguments/parameters are and how they relate to functions.

* Parameters are variables that hold the values we pass into functions and behave like local variables.

* Arguments are the values we pass to a function's parameters when we invoke the function.

###4 Describe/define mutating vs non-mutating functions. 

* Mutating Functions - Alter an existing object or data structure directly.

* Non-mutating Functions - Produce a new object or data structure.

### Using the `shoppingCart` variable, create a function that takes the `shoppingCart` variable and returns the total cost of both items as the `total` variable. `


```javascript

var shoppingCart = [20, 15];

function getTotalCost(prices) {
  let total = 0;
  for(i=0; i < shoppingCart.length; i++) 
    { 
    total += Number(shoppingCart[i]);
         } 
   console.log(total);
   return total; 
   
   }

getTotalCost(shoppingCart);


```