### what is `this` in JavaScript!?


```javascript
function print() {
  console.log(this.name);
}

var name = "Moein";
var obj1 = { name: "Yasin", print };
var obj2 = { name: "Mojtaba", print };

print(); //?
obj1.print(); //?
obj2.print(); //?
```

 > To understand this keyword, only we need to know how, when and from where the function is called, does not matter how and where function is declared or defined.
 
    So what if we use strict mode?! what happened to 'this'?