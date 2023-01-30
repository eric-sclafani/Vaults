**`Objects`** Key:value mappings denoted with `{}`. Similar to _python **dictionaries**_.
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