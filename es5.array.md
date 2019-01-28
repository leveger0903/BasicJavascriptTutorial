# ES5 陣列方法

> 參考網址: 
https://www.w3schools.com/jsref/jsref_obj_array.asp

## join
__將陣列以特定字元連接(類似 php 的 implode)__

````
var array  = ['Google', 'Apple', 'Facebook'];
var result = array.join(','); // 'Google Apple Facebook'
````

## slice
__取得部分陣列內容__

````
var array  = ['Google', 'Apple', 'Facebook'];
var result = array.slice(1, 3); // ['Apple', 'Facebook']
````

## indexOf
__找尋陣列是否有符合字符並回傳第一個位置, 未找到回傳 -1__

````
var array  = ['Google', 'Apple', 'Facebook', 'Apple'];
var result = array.indexOf('Apple'); // 1 
````

## lastIndexOf
__找尋陣列是否有符合字符並回傳最後一個位置,未找到回傳 -1__

````
var array  = ['Google', 'Apple', 'Facebook', 'Apple'];
var result = array.lastIndexOf('Apple'); // 3 
````

## pop
__拔掉陣列最後一個值__

````
var array  = ['Google', 'Apple', 'Facebook'];
array.pop(); // ['Google', 'Apple']
````

## shift
__拔掉陣列第一個值__

````
var array  = ['Google', 'Apple', 'Facebook'];
array.shift(); // ['Apple', 'Facebook']
````

## push
__插入值至陣列至最後一個位置__

````
var array  = ['Google', 'Apple'];
array.push('Facebook'); // ['Google', 'Apple', 'Facebook']
````

## unshift
__插入值至陣列至第一個位置__

````
var array  = ['Google', 'Apple'];
array.unshift('Facebook'); // ['Facebook', 'Google', 'Apple']
````

## reverse
__陣列順序翻轉__

````
var array  = ['Google', 'Apple', 'Facebook'];
array.reverse(); // ['Facebook', 'Apple', 'Google']
````

## sort
__陣列排序__

````
# 正排序
var array  = [2, 3, 1, 5, 4];
array.sort(); // [1, 2, 3, 4, 5]

# 逆排序
var array  = [2, 3, 1, 5, 4];
array.sort(function (a, b) {
  return b-a;
}); // [5, 4, 3, 2, 1]
````