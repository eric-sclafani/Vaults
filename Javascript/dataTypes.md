Types are `dynamic` in javascript.  There are 7 `primitive` data types

The `typeof` operator returns the datatype of an element
```js
typeof("Hello, world!") // 'String'
```
# String
## Properties
- `.length` - returns length of string
```js
let text = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";  
let length = text.length; //26
```
- `string[num]` - Can be used to access characters via indexing.
- Note:
	-   If no character is found, [ ] returns undefined, while charAt() returns an empty string.
	-   It is read only. str[0] = "A" gives no error (but does not work!)
## Methods
***(Italicized = optional parameter)***

----
- `.slice`(start, _stop_) - Returns a slice of a string (non-inclusive)
	- **Negative parameters** start the count from the end of string
```js
let text = "Apple, Banana, Kiwi";  
let part1 = text.slice(7, 13); // "Banana"
let part2 = text.slice(-5); // "Kiwi"
```
---
- `.substring`(start, *stop*) - Similar to `.slice`, except negative parameters are treated as 0
	- If start > _stop_, then .`substring` will swap those 2 arguments
```js
let str = "Apple, Banana, Kiwi";  
let part = str.substring(7, 13); // "Banana"
```
---
- `.replace`(old_string, new_string) - Replace a substring within a new substring
	- Returns a **new** string
	- Matches **once** by default
	- To change ALL instances in string, use `/g` regular expression tag
```js
let text = "Hi Hi Hi, World!";  
let newText1 = text.replace("Hi", "Hello"); // "Hello Hi Hi, World!"
let newText2 = text.replace(/Hi/g, "Hello"); // "Hello Hello Hello, World!"
```
---
- `.toUpperCase`(string) - Converts string to uppercase
```js
let text1 = "Hello World!";  
let text2 = text1.toUpperCase(); // "HELLO, WORLD!"
```
---
- `.toLowerCase`(string) - Converts string to lowercase
```js
let text1 = "Hello World!";  
let text2 = text1.toLowerCase(); // "hello, world!"
```
---
- `.concat`(string1, string2, ...) - Joins two or more strings
```js
let text1 = "Hello";  
let text2 = "World";  
let text3 = text1.concat(" ", text2); // "Hello World!"
```
---
- `.trim`() - Removes whitespace from both sides of string
- `.trimStart`() - Only trims the start
- `.trimEnd`() - Only trims the end
```js
let text1 = "      Hello World!      ";  
let text2 = text1.trim(); // "Hello World!"
let text3 = text1.trimStart(); // "Hello World!      "
let text4 = text1.trimEnd(); // "      Hello World!"
``` 
---
- `.padStart`(target_length, pad) - Pads start of string with a new string
- `.padEnd`(target_length, pad) - Pads end of string with a new string
```js
let text = "5";  
let padded1 = text.padStart(4,"x"); // "xxx5"
let padded2 = text.padEnd(4,"x"); // "5xxx"
```
---
- `.charAt`() - Returns the character at a specified index in a string
```js
let text = "HELLO WORLD";  
let char = text.charAt(0); // "H"
```
---
- `.charCodeAt`(index) - Returns unicode of a string character at an index position
```js
let text = "HELLO WORLD";  
let char = text.charCodeAt(0); // 72
```
---
- `.split`(element) - Converts a string into an array by splitting on a specified element
```js
text.split(",")    // Split on commas  
text.split(" ")    // Split on spaces  
text.split("|")    // Split on pipe
```
---
-  `.indexOf`(substring) -Returns index of the first occurence of a subtring 
-  `.lastIndexOf`(substring) -Returns the index of the last occurence of a subtring
	- Both methods accept a **second parameter** as the **starting position** for the search
```js
let text = "Please locate where 'locate' occurs!";  
text.indexOf("locate");// 7
text.lastIndexOf("locate");// 21
```
---
-  `.search`() - almost the same thing as `indexOf`, except it can also take regex
```js
let str = "Please locate where 'locate' occurs!";  
str.search(/locate/); // 7
```
-  `.match`() - 
-  `.matchAll`() - 
-  `.includes`() - 
-  `.startsWith`() - 
-  `.endsWith`() - 





---
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