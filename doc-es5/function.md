# ES5 方法

## 方法的型態

> 參考網址: http://www.w3schools.com/js/js_function_invocation.asp

- 全域方法: 會被視為視為 window 底下的物件

````
function saySomething (words) {
  return 'say: ' + words;
}

var a = saySomething('Hello World');
console.log(a);
````

- 高階方法: 將匿名方法傳到變數內, 可移除.

````
var method = function (words) {
  return 'say: ' + words;
}

var a = method('Hello World');
console.log(a);
````

- 高階方法: 建構物件, 將匿名方法傳到物件內其子元素, 可移除.

````
var object = {
  a: 123,
  b: 456,
  c: function (words) {
    return 'say: ' + words;
  }
}

var a = object.c('Hello World');
console.log(a);
````

- 方法中再包裝方法

````
function saySomething (concatFunc, words) {
  var content = '';
  for (var i in words) {
    content = concatFunc(content, words[i]);
  }

  return 'say: ' + content;
}

# 第一個參數通常被稱為閉包(Closure)
var a = saySomething(
  function (previousStats, words) {
    console.log(words);
    return previousStats + ' ' + words;
  },
  ['Hello', ',', 'how', 'are', 'you', '?'],
);

console.log(a);
````

- 方法在初始時被呼叫

````
(function (word) {
  console.log(word);
})('Hello');
````

## 方法撰寫建議

- 請不要將全域變數直接帶入方法內

````
# 不佳
var a = 123;
function saySomething () {
  return 'Hello, ' + a;
}

console.log(saySomething());

# 推薦
function saySomething (name) {
  return 'Hello, ' + name;
}

var a = '123';
console.log(saySomething(a));
````

- 用完即丟的區域變數請在方法內宣告

````
# 不佳
var sum;
function calc (a, b) {
  sum = a + b;
  return sum;
}

# 推薦
function calc (a, b) {
  var sum;
  sum = a + b;
  return sum;
}
````

- 執行完該方法, 建議均帶 return

````
# 不佳
function doSomething (a, b) {
  status = a && b;
}

doSomething(true, false);

# 推薦
function doSomething (a, b) {
  status = a && b;
  return status;
}

var status = doSomething(true, false);
````

- 可以自己需求引入高階方法