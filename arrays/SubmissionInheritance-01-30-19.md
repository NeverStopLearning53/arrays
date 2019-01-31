# **Exercises**
# **Questions**

##### **1 What does "DRY" stand for?  What does the "DRY principle" imply in programming or software development?**
"DRY" stands for "Don't repeat yourself" it implies using efficiencies and eliminating redundancies, programmers can make code more efficient and easy to change. At the heart of the "DRY principle" is the re-use of code modules. For instance, coding a repeatable task as a function means that function can be inserted and reused anywhere in the code, and does not have to be re-written for various calls. Benefits of using the "DRY Principle" include code readability and ease of maintenance.

#**Code Practice**
##### **Following the examples above, create a new prototype called Product and three instances of it. Each instance should be a separate product (for example, a shirt, a jacket, and a scarf).**

```
// Product will have type, color, price
function Product(type, color, price) {

    this.type = type;
    this.color = color;
    this.price = price;
}
// methods
Product.prototype.introduce = function() {
    console.log('This is a ' + this.color + " " + this.type + ' and it costs $' + this.price + ' dollars.');
  };

var shirt = new Product('shirt', 'blue', 15);
var jacket = new Product('jacket', 'violet', 25);
var scarf = new Product('scarf', 'red', 30);
shirt.introduce(); //
jacket.introduce(); //
scarf.introduce(); //
```

