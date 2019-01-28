#ES5 URI 方法

> 參考網址: 
https://www.w3schools.com/jsref/obj_location.asp

## protocol
__當前 URI 通訊協定__

````
location.protocol; // https:
````

## host
__當前 URI 網域__

````
location.host; // tw.yahoo.com
````

## port
__當前 URI 埠值__

````
location.port; // 443
````

## pathname
__當前 URI 路徑__

````
location.pathname; // /folder/filename.php
````

## search
__當前 URI Query值__

````
location.search; // ?app_id=1&app_name=yahoo 
````

## hash
__當前 URI 頁面錨點__

````
location.hash; // #tag
````

## href
__完整頁面資訊__

````
location.href; // https://tw.yahoo.com/filename.php?app_id=1#tag
````
----

## reload
__重新載入頁面__

````
location.reload();
````

## replace
__網址重新導向, 但不記錄於歷史__

````
location.replace('https://www.google.com');
````

## assign
__網址重新導向, 但紀錄於歷史__

````
location.assign('https://www.google.com');
````
