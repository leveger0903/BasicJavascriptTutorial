# ES5 AJAX

## 步驟說明
- 先宣告 ajax 物件

````
var request = new XMLHttpRequest();
````

- 建立 onreadystatechange 事件監聽 ajax 狀態

````
request.onreadystatechange = function() {
  switch(request.readyState) {
    case 4:
      if (request.status == 200)
        document.getElementById("my_text").innerHTML = request.responseText;
      else 
        document.getElementById("my_text").innerHTML = "Request Failed";
        break;

      default:
        document.getElementById("my_text").innerHTML = "Waiting ...";
  }
};
````

- open('http方法', '請求網址', 是否同步傳輸);

````
request.open("GET", "data.txt", true);
````

- send()建立請求

````
request.send();
````

## 完整範例

````
function loadAjax() {
  var request = new XMLHttpRequest();

  request.onreadystatechange = function() {

    switch(request.readyState) {
      case 4:
        if (request.status == 200)
          document.getElementById("my_text").innerHTML = request.responseText;
        else 
          document.getElementById("my_text").innerHTML = "Request Failed";
      break;

      default:
        document.getElementById("my_text").innerHTML = "Waiting ...";
    }
  };

  request.open("GET", "data.txt", true);
  request.send();
}
````