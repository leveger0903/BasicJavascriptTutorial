# ES5 瀏覽器方法

> 參考網址: 
https://www.w3schools.com/jsref/obj_navigator.asp

## cookieEnabled
__是否允許使用cookie__

````
navigator.cookieEnabled; // true
````

## geolocation
__取得地理定位__

````
if (navigator.geolocation) {
  navigator.geolocation.getCurrentPosition((pos) => {
    console.log("geo status: " + pos.coords.latitude + "," + pos.coords.longitude);
  });
}
````

## language
__取得語系__

````
navigator.language; // zh-TW
````

## online
__取得連線狀態__

````
navigator.online; // true
````

## userAgent
__取得瀏覽器資訊__

````
navigator.userAgent; // Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.110 Safari/537.36
````