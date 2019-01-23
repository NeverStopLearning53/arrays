# **Exercises**
# **Questions**

##### **1. What is the difference between `document.querySelector()` and `document.querySelectorAll()`?**
The `querySelector()` and `querySelectorAll()` both allow you to pass multiple selectors for your query. The main difference between the two is that `querySelector` returns a reference to the _first_ element ift finds which matches the query, while `querySelectorsAll()` retruns an array-like object of all matches.
##### **2. What is the difference between `getElement(s)By` and `querySelector(All)`?**
The difference is that the "getElement(s)By" methods are often faster in the browser and are preferred when possible. If you need more flexibility then use `querySelector()` or `querySelectorAll()`.

##### **3. What do JavaScript event handlers do and what is an example of one?**
Javascript event handlers are a set of functions which "handle" what happens when an event is triggered?

Examples of Event Handlers are 

* The user clicks an HTML element ("onclick")
* The browser has finished loading the page ("onload")
* The user moves the mouse moves over an HTML element ("onmouseover")
* An HTML element has been changed ("onchange")

# **Code Practice**
##### **Using the code from the prior checkpoint, add an Event Handler to the `<li>` element and `console.log()` the name of the shirt they selected.**

```html

<!DOCTYPE html>
<html>
<head>
	<title></title>
</head>
<body>
	<h3>Shirts</h3>
	<ul id='list'>
    	<li onclick="selected('Biker Jacket')">Biker Jacket</li>
    	<li onclick="selected('Mens Shirt')">Mens Shirt</li>
	</ul>

	<script>
			

		function selected(message) {

			console.log(message + " Selected");

		}

			


</script>

</body>
</html>

```