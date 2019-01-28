# ES5 變數

## 基本變數型態

> 參考網址: http://www.w3schools.com/js/js_datatypes.asp

- 數字型態 (number)

````
var a1 = 123;
console.log(typeof a1); // number
````

- 文字型態 (string)

````
var a2 = "123";
console.log(typeof a2); // string
````

- 陣列 / 物件 (array / object)

````
var a3 = [123, 456, 789];
console.log(typeof a3); // object

var a4 = { a: 123, b: 456 };
console.log(typeof a4); // object
````
- 布林值 (true / false)

````
var a5 = true;
console.log(typeof a5); // boolean
````

## 變數呼叫

> 參考網址: http://www.w3schools.com/js/js_scope.asp

- 全域變數:  
  全域變數任何位置都可呼叫(包含在function內),  
  但實作上儘量少用全域變數.

````
var a2 = 1;

function test () {
  console.log(a2); // 1
}

test();
console.log(a2); // 1
````

- 區域變數:  
  區域變數通常放在function內,  
  通常執行完funtion即會被銷毀.

````
var a2 = 1;

function test () {
  var b2 = 2;
  console.log(b2); // 2
}

test();
console.log(b2); // Uncaught ReferenceError: b2 is not defined
````

## 變數串接與計算

> 參考網址: http://www.w3schools.com/js/js_syntax.asp

- 兩個數值相加, 得到數值

````
var a = 1;
var b = 2;
var result = a + b;

console.log(typeof a); // number
console.log(typeof b); // number
console.log(typeof result); // number: 3
````

- 兩個字串串接

````
var a = '1';
var b = '2';
var result = a + b;

console.log(typeof a); // string
console.log(typeof b); // string
console.log(typeof result); // string: 12
````

- 不同型態串接, 可能無法預期結果, 不建議.

````
var a = '1';
var b = 2;
var result = a + b;

console.log(typeof a); // string
console.log(typeof b); // number
console.log(typeof result); // string: 12

var a = undefined;
var b = 2;
var result = a + b;

console.log(typeof a); // undefined
console.log(typeof b); // number
console.log(typeof result); // NaN: 不是數字
````

- 型態不同, 建議先轉換成相同的型態

````
var a = '1';
var b = 2;

var result = parseInt(a) + b;
console.log(typeof result); // number: 3

var result = a + b.toString();
console.log(typeof result); // string: 12
````

- 連續的字串串接

````
var a = 'How ';
var b = 'are ';
var c = 'you?';

var result = a + b;
var result = result + c;

console.log(result); // How are you?

# 相當於
var result = a;
result += b;
result += c;
console.log(result); // How are you?
````