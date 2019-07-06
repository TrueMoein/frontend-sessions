## Closure
A closure is the **combination** of a function and the **lexical environment** within which that function was declared. :shit:


#### Lexical scoping

The word "lexical" refers to the fact that lexical scoping uses the **location** where a variable is declared within the source code to determine where that variable is available. Nested functions have access to variables declared in their outer scope

Always remember=> **Lexical environment = backpack**

A closure is the combination of a function and the lexical environment within which that function was declared. This environment consists of any local variables that were in-scope at the time the closure was created


#### Module pattern in old days
Get familiar [here](https://coryrylan.com/blog/javascript-module-pattern-basics)

#### Practice

<div dir="rtl">
تابع foo را به نحوی بنویسید که با که با هربار اجرای keepSquare در صورتی که مقدار قبلی ورودی این تابع با مقدار جدید یکسان باشد خروجی فراخوانی قبل را برگرداند. 
</div>


```javascript
   function square(x) {
     return x ** 2;
   }
   
   const keepSquare = foo(square);

   keepSquare(10);
   keepSquare(10);
```


<div dir="rtl">تابع calc را پیاده‌سازی کنید</div>


```javascript
    calc('+')(1)(2); // 3
    calc('*')(2)(3); // 6
```


<div dir="rtl"> با استفاده از closure ها مشکل زیر را حل کنید.</div>

```javascript
    ['10', '20', '30'].map(parseInt); // [1, NaN, NaN]
```
