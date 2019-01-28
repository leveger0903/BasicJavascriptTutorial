# ES5 數學方法

> 參考網址: 
https://www.w3schools.com/jsref/jsref_obj_math.asp

## abs
__返回絕對值__

````
var num = -100;
num = Math.abs(num); // 100
````

## ceil
__無條件進位__

````
var num = 99.3;
num = Math.ceil(num); // 100
````

## floor
__無條件捨去__

````
var num = 100.7;
num = Math.floor(num); // 100
````

## round
__數字四捨五入__

````
var num = 100.3;
num = Math.round(num); // 100
````

## max
__取得最大值__

````
var array = [1, 5, 9];
var num = Math.max(...array); // 9
````

## min
__取得最小值__

````
var array = [1, 5, 9];
var num = Math.min(...array); // 1
````

## random
__亂數取得 0 ~ 1 內的數字__

````
var num = Math.random();
````