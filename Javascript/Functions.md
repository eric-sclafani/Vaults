----
### getElementbyId()
- Accesses an HTML element by an **id**
```js
// retrieves HTML element with the id "demo"
document.getElementById("demo"); 
```
----
###  .innerHTML()
- Writes into an HTML element
```js
// changes "demo" HTML element content to "Hello, world!"
document.getElementById("demo").innerHTML = "Hello, world!";
```
----
###  document.write() 
- Write into the HTML output
- <font style="color:violet">NOTE</font>: Never call `document.write` after the document has finished loading. It will overwrite the whole document
```js
// write "11" to document
document.write(5 + 6);
```
----
### window.alert()
-  Write into an alert box
```js
// alert user with message "11"
window.alert(5 + 6);
```
---OR---
```js
alert(5 + 6); // window is the global scope, so it can be ommitted here
```
---
### console.log()
- Write into the browser console
```js
// writes "11" to browser console (open with F12)
console.log(5 + 6);
```
----
### window.print()
- Method called in the browser to print content of current window
```HTML
<button onclick="window.print()">Print this page</button>
```
----
