### what is `this` in JavaScript!?


```javascript
function print() {
  console.log(this.name);
}

var name = "Ninja";
var obj1 = { name: "Yasin", print };
var obj2 = { name: "Mojtaba", print };

print(); //?
obj1.print(); //?
obj2.print(); //?
```