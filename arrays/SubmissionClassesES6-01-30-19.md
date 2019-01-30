# **Exercises**
# **Questions**

##### **1 What is object-oriented programming?**
Using objects to model real world things that we want to represent inside our programs and/or provide a simple way to access functionality that would otherwise be hard or impossible to make use of.
##### **2 What is a constructor?**
It is a method, a special method, called when creating and initializing a class. There can be only one `constructor` within the class.

##### **3 What is the purpose of the keyword `super`**
The **super** keyword is used to access and call functions on an object's parent. The `super.prop` and `super[expr]` expressions are valid in any method definition in both classes and object literals. When used in a construtor the `super` keyword appears alone and must be used before the `this` keyword is used. The `super` keyword can also be used to call functions on a parent object.

##### **4 What are classes that do not use the keyword `extends` called?**
The class from which the subclass is derived(or a class which does not use the keyword 'extends` is called a superclass (also a base class or a parent class).

#**Code Practice**
##### **Using the `Clothes` class we previously created, create a `Shirt` class that `extends` the `Clothes` class. Don't forget the `super().`**

```
var Clothes = class {
    constructor(name, size, price){
        this.name = name;
        this.size = size;
        this.price = price;      

    }
}
// add code below
class Shirt extends Clothes {
 constructor(name, size, price) {
    super(name, size, price); // call the super class constructor and pass in the name parameter
 }
    type() {
    console.log(this.name, this.size, this.price);
  }
}

let s = new Shirt('Dress Shirt', '14', '25');
s.type(); // Dress Shirt
```

