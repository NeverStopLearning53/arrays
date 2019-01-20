# **Exercises**
# **Questions**

##### **1. In your own words, what is a JavaScript object?**

Objects are values that can contain other values. They use keys to name values, which are a lot like variables.

##### **2. What is a property of a JavaScript object?**

Properties are the most important part of any JavaScript object.  Properties are the values associated with a JavaScript object.


```javascript

// //declare a class called `clothes` that takes three parameters in the constructor, `name`, `size`, and `price`.
// create a variable called `shirt` that is equal to a new instance of Clothes with name = V-Neck, size = 'Medium' and price = // 20

class Clothes {
  constructor(name, size, price) {
    this.name = name;
    this.size = size;
    this.price = price;  
  }
}
let shirt = new Clothes('V-Neck', 'Medium', 20 );
console.log(shirt.name,shirt.size,shirt.price);

```