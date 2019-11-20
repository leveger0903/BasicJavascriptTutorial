# ES5 全域方法

## encodeURI
__編碼特殊字元為UTF-8編碼(不包含+#$,:;=?)__

````
var text = 'https://www.google.com?q=選舉';
encodeURI(text); // https://www.google.com?q=%E9%81%B8%E8%88%89
````

## decodeURI
__解碼特殊字元為UTF-8編碼__

````
var text = 'https://www.google.com?q=%E9%81%B8%E8%88%89';
decodeURI(text); // https://www.google.com?q=選舉
````

## encodeURIComponent
__編碼特殊字元為UTF-8編碼(包含+#$,:;=?)__

````
var text = 'https://www.google.com?q=選舉';
encodeURIComponent(text); // https%3A%2F%2Fwww.google.com%3Fq%3D%E9%81%B8%E8%88%89
````

## decodeURIComponent
__解碼特殊字元為UTF-8編碼__

````
var text = 'https%3A%2F%2Fwww.google.com%3Fq%3D%E9%81%B8%E8%88%89';
decodeURIComponent(text); // https://www.google.com?q=選舉
````

## parseFloat
__轉換成浮點數__

````
var num = '100.7';
parseFloat(num); // 100.7
````

## parstInt
__轉換成整數__

````
var num = '100.7';
parseInt(num); // 100
````

## toString
__轉換成字串__

````
var num = 100.7;
num.toString(); // '100.7'
````

## btoa
__base64編碼__

````
var text = 'Hello World.';
btoa(text); // SGVsbG8gV29ybGQu
````

## atob
__base64解碼__

````
var text = 'SGVsbG8gV29ybGQu';
atob(text); // 'Hello World.'
````

## sessionStorage.setItem
__以 key/value 方式儲存資料(關閉分頁即消失)__

````
sessionStorage.setItem('name', 'kaoru');
````

## sessionStorage.getItem
__以 key/value 方式取得資料(關閉分頁即消失)__

````
sessionStorage.getItem('name');
````

## localStorage.setItem
__以 key/value 方式儲存資料(清空 cache 消失)__

````
localStorage.setItem('name', 'kaoru');
````

## localStorage.getItem
__以 key/value 方式取得資料(清空 cache 消失)__

````
localStorage.getItem('name');
````


