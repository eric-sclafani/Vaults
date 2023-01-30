Types are `dynamic` in javascript.  There are 7 `primitive` data types

The `typeof` operator returns the datatype of an element
```js
typeof("Hello, world!") // 'String'
```

# Primitives
## String


## Number  
All numbers are stored as `demimals`, but can be written with or without decimal places:
```js
typeof(45) // 'number'
typeof(32.21) // 'number'
```
Really **large** or **small** numbers can be written using `exponential notation`:
```js
let y = 123e5;    // 12300000  
let z = 123e-5;   // 0.00123
```
## Bigint
Bigint's are for numbers too large to represent with javascript's normal `Number` type
```js
let x = BigInt("123456789012345678901234567890");
```
## Boolean
`true` or `False`
```js
let x = 5;  
let y = 5;  
let z = 6;  
(x == y)       // Returns true  
(x == z)       // Returns false
```
## Undefined
Variables created without a value are given the `undefined` type.
```js
let car;    // Value is undefined, type is undefined
let bus = undefined;    // Value is undefined, type is undefined
```
## Null
## Symbol


# Non-primitives
## [[Objects]]

## array 
Similar to _python **lists**_.  Denoted with square brackets and separated by commas
```js
const cars = ["Saab", "Volvo", "BMW"];
```
## date