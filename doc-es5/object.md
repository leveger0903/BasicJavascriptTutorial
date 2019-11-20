# ES5 物件/陣列/迴圈

## 宣告陣列的方法

````
var array = new Array();
````

或是

````
var array = [];
````

## 陣列第一個索引值為 0

````
var array = [1, 4, 9, 16, 25, 36];

# 由左開始算(第一個索引值為 0 ), 相當於第 6 個索引值
array.push(49);
````

## 取用陣列的方式
````
var array = [1, 4, 9, 16, 25];

console.log(array[0]);
console.log(array[2]);
console.log(array[4]);
````

## 宣告物件的方法

````
var object = new Object();
````

或是

````
var object = {};
````

## 物件內新增屬性方法

````
var object = { a: 1, b: 4, c: 9 };
object.d = 16;
````

或是

````
object['d'] = 16;
````

## 取用陣列的方式

````
var object = { a: 1, b: 4, c: 9 };
console.log(object.c);
````

或是

````
console.log(object['c']);
````

## 迴圈類型

- for ...

````
for (var i = 1; i <= 5; i++) {
  console.log('for loop:' + i);
}
````

- for ... in ...\
類似於 php 的 foreach

````
var array = [1, 4, 9, 16, 25];
for (var i in array) {
  console.log('index:' + i + ' value:' + array[i]);
}
````

- while ... do ...\
判斷符合條件執行

````
var i = 0;
while (i < 5) {
  console.log('for loop:' + i);
  i++;
}
````

- do ... while ...\
執行後再做判斷是否符合條件

````
var i = 0;
do {
  console.log('for loop:' + i);
  i++;
} while (i < 5)
````
