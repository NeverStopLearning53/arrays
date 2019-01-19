# **Exercises**
# **Questions**
##### **1 Describe the `map()` function.**

The `map()` function iterates over each item in the array, transforming it and returning a new array. The `map()` function does not modify the original array.

##### **2 Describe the `filter()` function.**

The `filter()` function iterates over each item in an array and keeps items when the condition is true.

##### **3 What is the difference between the `map()` and `filter()` functions?**

 _The `map()` function changes each and every item in the array and returns those changes in a new array._
 _The `filter()` function *only* applies changes to items in the array when the condition is true(in this sense it applies a filter to the array and only applies the changes to those items where the condition is true) and returns those changes in a new array._



# **Code Practice**

##### **Using the numbers provided in the editor, use the `filter()` function to keep any numbers that are greater than three, then use the `reduce()` function to sum the filtered numbers.**

_The code editor does not save code; it is a playground. If you leave the page, close the window, etc., it will not keep your work. Be sure to copy/paste your answers/code into the submission box below!_


```javascript

var numbers = [1,2,3,4,5,6,7,8,9,2,3,4,5,6,1,2,3,4,5,6,7,8,8,4,3,2];
var total = numbers
.filter(item => item < 3) // returns [1,2,2,1,2,2]
.reduce((total, item) => total + item); // returns 10
console.log(total); // logs 10

```
