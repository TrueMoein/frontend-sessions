### what is `this` in JavaScript!?

```javascript
function print() {
  console.log(this.name);
}

const name = "Moein";
const obj1 = { name: "Yasin", print };
const obj2 = { name: "Mojtaba", print };

print(); //?
obj1.print(); //?
obj2.print(); //?
```

 > To understand this keyword, only we need to know how, when and from where the function is called, does not matter how and where function is declared or defined.
 
    So what if we use strict mode?! what happen to 'this'?
    
### What is "Default" and "Implicit" binding of `this`?

- If we are in strict mode then the default value of this keyword is undefined otherwise this keyword act as global object, it’s called default binding of this keyword. (default is window object in case of browser).
- when there is an object property which we are calling as a method then that object becomes this object or execution context object for that method, it is implicit binding of this keyword.

```javascript
const obj1 = {
  name: "Moein",
  print() {
    console.log(this.name);
  }
}
const name = "Mojtaba";
const obj2 = { name: "Yasin", print: obj1.print };
const print = obj1.print;

print(); // Default binding - ??
obj1.print(); // Implicit binding - ??
obj2.print(); // Implicit binding - ??
```

### "Explicit" and "Fixed" Binding of `this` keyword

 - If we use `call` and `apply` method with calling function, both of those methods take as their first parameter as execution context. that is `this` binding.
 
  #### Explicit
 ```javascript
function print() {
  console.log(this.name);
}

const name = "Mojtaba";
const obj = { name: "Yasin" }

print();           // ?
print.call(obj);   // ?
```

#### Fixed or Hard binding of `this`:

```javascript
let print = function() {
  console.log(this.name);
}
const name = "Moein";
const obj1 = { name: "Mojtaba" };
const obj2 = { name: "Yasin" };

const originalPrintFunc = print;
print = function() {
  originalPrintFunc.call(obj1);
};

print();           // ??
print.call(obj2);  // ??
```

### Our Own Bind Implementation

Function.prototype.bound = function(context) {
  const fn = this;
  
  return function(...args) {
    fn.call(context, ...args)
  }
}
