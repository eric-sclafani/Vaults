# Objects
**`Objects`** Key:value mappings denoted with `{}`. Kind of similar to _python **dictionaries**_.
```js
const person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};
person.firstName // "John"
person.lastName // "Doe"
person.eyeColor // "blue"
```
- It is common practice to declare `objects` using `const`
- The **key:values** pairs in JavaScript objects are called `properties`
# Object methods
- Objects can also have `methods`
- Methods are **actions** that can be performed on objects.
- Methods are stored in properties as **function definitions**.
```js
const person = {  
  firstName: "John",  
  lastName : "Doe",  
  id       : 5566,  
  fullName : function() {  
    return this.firstName + " " + this.lastName;  
  }  
};
```
# this
The "`this`" keyword refers to whatever object is being invoked at the time.
1. In an object method, `this` refers to the **object**.
2. Alone, `this` refers to the **global object**.
3. In a function, `this` refers to the **global object**.
4. In a function, in strict mode, `this` is `undefined`.
5. In an event, `this` refers to the **element** that received the event.
6. Methods like `call()`, `apply()`, and `bind()` can refer `this` to **any object**.