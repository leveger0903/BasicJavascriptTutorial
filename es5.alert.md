# ES5 Window方法

> 參考網址: 
http://www.w3schools.com/jsref/obj_window.asp

## alert
__通知視窗__

````
alert('hello world');
````

## confirm
__確認視窗__

````
var ask = confirm('choose one');

if (ask == true)
  alert('you choose OK');
else
  alert('you choose Cancel');
````

## prompt
__提示字元視窗__

````
var ask = prompt('請輸入內容', '預設內容');

if(ask != null)
  alert(ask);
````

## open
__開啟視窗__

````
var popup = window.open(
  'https://google.com', 
  'popup',
  'width=1024, height=600' 
);
````

## close
__關閉視窗__

````
popup.close(); 
````

## print
__進行列印__

````
window.print();
````