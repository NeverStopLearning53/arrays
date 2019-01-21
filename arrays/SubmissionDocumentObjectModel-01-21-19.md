# **Exercises**
# **Questions**

##### **1. What does the acronyn DOM stand for and explain in your own words what is is.**

DOM stands for Document Object Model. 

The HTML DOM is an API (Programming Interface) for JavaScript:

* JavaScript can add/change/remove HTML elements
* JavaScript can add/change/remove HTML attributes
* JavaScript can add/change/remove CSS styles
* JavaScript can react to HTML events
* JavaScript can add/change/remove HTML events

Objects are values that can contain other values. They use keys to name values, which are a lot like variables.

##### **2. How does the DOM make web programming more efficient?**
The DOM means that the browser evaluates the entire HTML document as a single Javascript object. This object also gets special methods added to it to help find each element or a group of elements within the object. This makes web programming way more efficient.
# **Code Practice**
##### **Using `createElement` and `getElementById.` Add a new Shirt to the `ul`. Set the `innerText` equal to 'Mens T-shirt'.**

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Using Javascript Add Items to an unordered list.</title>
</head>
<body>

    <h3>Shirts</h3>
	<ul id="dynamic-list">
    	<li>Biker Jacket</li>
	</ul>

    <script>
		function addItem(itemName) {
			
			var ul = document.getElementById("dynamic-list");
			var li = document.createElement("li");
			li.setAttribute('class', 'item');
			li.innerText=itemName;
			ul.appendChild(li);
			
		}
		addItem("Men's T-Shirt");

		addItem("Women's T-Shirt");

		addItem("Unisex T-Shirt");

		addItem("Seahawks Sweatshirt");


    </script>
</body>
</html>

```