# ES5 判斷子

## 判斷子

- ==
- ===
- !=
- !==
- \>
- \<
- \>=
- \<=

## 潛比較(不包含型態)

- 以下均為 true

````
var a = true; // boolean, true
var b = 1; // number, true
var c = "1"; // string, true
var d = 1; // number, true
````

- 以下均為 false

````
var a = false; // boolean, true
var b = 0; // number, true
var c = "0"; // string, true
var d = 0; // number, true
````

````
console.log(true == 1);  // true
console.log(false == 0); // true
````

## 深比較(包含型態均需要一致)

````
console.log(true === 1);  // false
console.log(false === 0); // false
````