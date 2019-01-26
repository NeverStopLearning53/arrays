# **Exercises**
# **Questions**

##### **1. Open your browser. Open up Chrome DevTools. Click on the Network tab on DevTools. Go to your bloc dashboard page. What Request Urls is Bloc using to get your information from the API?**
* https://api.segment.io/v1/t
* https://api.segment.io/v1/p
* https://api.segment.io/v1/i

##### **2. Where can I find the cookies being used on the webpage using the Chrome DevTools?**
Open up Chrome DevTools ... click application ... click on cookies ... then see dropdown with website listed .. click on website and you will see list of cookies display to the right.

##### **3. Where can you execute JavaScript in the DevTools?**
Use the Console Tab.

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
    		<li>Biker Jacket</li>
    		<li>Mens Shirt</li>
	</ul>

<script>
			
const listTag = document.getElementsByTagName('li');

for (i=0; i < listTag.length; i++) {
listTag[i].addEventListener('click', function(){
  
  console.log('You Selected a ', this.innerHTML);
  });
}

		
</script>
</body>
</html>
```