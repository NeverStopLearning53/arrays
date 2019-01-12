# **Exercises**
## **Questions**
###1 What are the three types of conditional statements?

*The three types of conditional statements are `if`, `else` and `elseif`*


###2 What are four types of comparison operators and how you would use them? 

I actually have listed out 8 comparison operators. I would use them in logical statements to determine equality or difference between variables or values.

The **equality operator** `==` compares two values and returns `true` if they are equivalent or `false` if they are not. With the **equality operator**, JavaScript will convert the `string` and `number` data types to be the same.

The **strict equality operator** `===` is similar to the **equality operator**, however, strict equality tests both the value _and_ the data type. _Strict equality will not convert data types._

The **inequality operator** `!=` is the opposite of the equality operator. It checks if two values are "Not Equal" and returns `true` when the **equality operator** would return `false`. Just like the **equality operator**, the **inequality operator** _will convert data types of values while comparing._

The **strict inequality operator** `!==` is the opposite of the **strict equality operator**. It means "Strictly Not Equal" and returns `false` where strict equality would return  `true`. _Strict inequality will not convert data types._

The **greater than operator** `>` compares two numbers. When the number on the left is greater than the number on the right, it returns `true`. Otherwise, it returns `false`. _Just like the **equality operator**, the **greater than operator** will convert data types of values while comparing._

The **less than operator** `<` compares two numbers. If the left number is less than the right number, it returns `true`. Otherwise, it returns `false`. _Just like the **equality operator**, the **less than operator** will convert data types of values while comparing._

The **greater than or equal to operator** `>=` compares two numbers. If the number on the left is greater than or equal to the number on the right, it returns `true`. Otherwise, it returns `false`. _Just like the **equality operator**, the **greater than or equal to operator** will convert data types of values while comparing._

The **less than or equal to operator** `<=` compares two numbers. If the number on the left is less than or equal to the number on the right, it returns `true`. When the number to the left is greater than the number to the right, it returns `false`. _Just like the **equality operator**, **the less than or equal to operator** will convert data types of values while comparing._

## **Code Practice**

### Create a variable called grade and set it to the grade you plan to receive on this assignment. Then write an if statement that will check whether the grade is equal to an A, B, C, D, or F and inform the user if they passed or failed using console.log().

```javascript

let grade = 'A';

if (grade == 'A') { // you need to get a "C" or "B" or "A" to pass

console.log("You passed!");

} else if (grade == 'B') { // you need to get a "C" or "B" or "A" to pass

console.log("You passed!");

} else if (grade == 'C') { // you need to get a "C" or "B" or "A" to pass

console.log("You passed!");

} else { // if you get a "D" or "F" you have failed the assignment

console.log("You failed!");
}

```