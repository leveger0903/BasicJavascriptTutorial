# ES5 字串方法

> 參考網址: 
https://www.w3schools.com/jsref/jsref_obj_string.asp

## length
__返回字串長度__

````
var str = 'hello world';
console.log(str.length); // 11
````

## replace
__搜尋並取該部分字串__

````
var str = 'hello world';
str = str.replace('world', 'kelly'); // hello kelly
````

## slice
__取得字串一部分(第 n 字開始到第 m 字結束)__

````
var str = 'hello world';
str = str.slice(6, 11); // world
````

## split
__以指定字元作為依據將字串分割為陣列__

````
var str = 'hello world';
str = str.split(' '); // ['hello', 'world']
````

## substr
__取得字串一部分(第 n 字開始向後取 m 個字)__

````
var str = 'hello world';
str = str.substr(6, 5); // world
````

## toLowerCase
__將字串轉為小寫__

````
var str = 'HELLO WORLD';
str = str.toLowerCase(); // hello world
````

## toUpperCase
__將字串轉為大寫__

````
var str = 'hello world';
str = str.toUpperCase(); // HELLO WORLD
````

## toString
__將變數型態轉為字串__

````
var num = 12345;
num = num.toString(); // '12345'
````
## indexOf
__搜尋字串關鍵字(找不到顯示-1)__

````
var str = 'hello world';
str = str.indexOf('world'); // 6
````

## trim
__將字串左右空白去除__

````
var str = ' hello world ';
str = str.trim(); // 'hello world'
````