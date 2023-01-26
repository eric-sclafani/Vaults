# Purpose
This directory contains notes on `Javascript` for the purposes creating `D3` visualizations for CSE 564. 
Below is my goal:
![[goal.jpg | 500]]
# Code blocks
Javascript statements can be grouped together in `code blocks` using curly braces `{}`
```js
function myFunction() {  
  document.getElementById("demo1").innerHTML = "Hello Dolly!";  
  document.getElementById("demo2").innerHTML = "How are you?";  
}
```
# Variable declaration
The three keywords for defining variables are `var`, `let`, and `const`. They have their own sets of constraints:
|                               | var      | let   | const |
|-------------------------------|----------|-------|-------|
| Scope                         | function | block | block |
| Hoisting?                     | Yes      | No    | No    |
| Allows value reassignment?    | Yes      | Yes   | No    |
| Allows variable reassignment? | Yes      | No    | No    |
