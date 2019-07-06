- closure

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