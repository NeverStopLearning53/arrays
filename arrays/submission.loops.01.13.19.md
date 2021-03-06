#**Exercises**
###**Questions**
### What are the three things you need to provide for a loop? I.e., in `for(a ; b ; c){}`, what are a, b, and c?

* a _initialization_-where the initial condition of the loop is setup.

* b _condition_-where Javascript checks the condition before each iteration of the loop. If the condition evaluates to `true`, the loop will continue to run, if not, the loop will stop.

* c _final-expression_-this runs after each iteration of the loop. It is the job of the final-expression to change the condition so that the loop eventually stops.

###**Describe infinite loops and how to avoid them.**
_Infinite Loop_ - This occurs when the condition of the loop is always true, so the loop never stops. Infinite loops can freeze or crash your computer. Writing and testing your final-expression making sure the loop stops is extremely important to making sure you don't have an _infinite loop_.

```javascript

var shoppingCart = [
  {
      id: 0,
      name: 'Mens Shirt',
      price: 20,
      size: 'Large'
  },
  {
  id: 1,
  name: 'kids shirt',
  price: 15,
  size: 'small'
}
]

for (var i = 0; i < shoppingCart.length; i++) {
    console.log(shoppingCart[i].name);
}
```