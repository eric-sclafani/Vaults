# Events
An `HTML event` can be something the browser does, or something a user does.
Here are some examples of HTML events:
1.   An HTML web page has finished loading
2.  An HTML input field was changed
3.   An HTML button was clicked
# Event handling
HTML allows event handler attributes, **with JavaScript code**, to be added to HTML elements

The following snippet writes a Date to the "demo" HTML element when a button is clicked
```html
<html>
	<body>
		<button onclick="document.getElementById('demo').innerHTML=Date()">The time is?</button>
	<p id="demo"></p>
	</body>
</html>
```
The following snippet changes the button object itself, with `this` referring to the element. 
```html
<html>
<body>
<h2>JavaScript HTML Events</h2>
<button onclick="this.innerHTML=Date()">The time is?</button>
</body>
</html>
```
Often times, events are Javascript functions:
```html
<html>
	<body>
		<h2>JavaScript HTML Events</h2>
		<p>Click the button to display the date.</p>
		<button onclick="displayDate()">The time is?</button>
		<script>
		function displayDate() {
		  document.getElementById("demo").innerHTML = Date();
		}
		</script>
		<p id="demo"></p>
	</body>
</html> 
```
# Common HTML Events
Here is a list of common events:
![[html_events.jpg]]