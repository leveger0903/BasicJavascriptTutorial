# ES5 時間方法

## setTimeout
__設定倒數計時器__

````
var timeout = setTimeout(function () {
  console.log('hello world');
}, 2000);
````

## clearTimeout
__清除倒數計時器__

````
clearTimeout(timeout);
````

## setInterval
__設定間隔計時器__

````
var interval = setInterval(function () {
  console.log('hello world');
}, 2000);
````

## clearInterval
__清除間隔計時器__

````
clearInterval(interval);
````