----
# Purpose
This directory contains notes on `Javascript` for the purposes creating `D3` visualizations for CSE 564. 
Below is my goal:
![[goal.jpg | 500]]

-----
# Javascript
- A `javascript` program is a series of statements that get executed to interact with a webpage (HTML & CSS)
- Statements are separated by `semicolons` ;
- `camelCase` is the standard naming scheme
---
# Code blocks
Javascript statements can be grouped together in `code blocks` using curly braces `{}`
```js
function myFunction() {  
  document.getElementById("demo1").innerHTML = "Hello Dolly!";  
  document.getElementById("demo2").innerHTML = "How are you?";  
}```
---
# Variable declaration
The three keywords for defining variables are `var`, `let`, and `const`. They have their own sets of constraints:
|                               | var      | let   | const |
|-------------------------------|----------|-------|-------|
| Scope                         | function | block | block |
| Hoisting?                     | Yes      | No    | No    |
| Allows value reassignment?    | Yes      | Yes   | No    |
| Allows variable reassignment? | Yes      | No    | No    |

## Var
- `var` was primarily used from 1995 - 2015. Use `var` when your code must be ran in old browsers

## let & const
- <font style="color:violet">General rule</font>: always declare variables with `const`. If the value of your variable may change, use `let`
```js
const price1 = 5;  
const price2 = 6;  
let total = price1 + price2;```
- Variables can be declared spanning multiple lines:
```js
let person = "John Doe",  
    carName = "Volvo",  
    price = 200;
```

## Undefined
Variables declared without an explicit value will have the `undefined` value
```js
let carName;
```

---
# Comments
- Single line comment start with `//`
- Multiline comments start with `/*`, end with `*/`
---