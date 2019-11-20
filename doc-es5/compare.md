# ES5 判斷式

- if ... else ...

````
# 標準寫法
if (status == true) {
  console.log('status: true');
} else {
  console.log('status: false');
}
````

````
# 判斷式內僅有一行程式碼時, 可省略花括號
if (status == true)
  console.log('status: true');
else
  console.log('status: false');
````

````
# 承上一章節, 潛比較書寫方式
if (status) // true
  console.log('status: true');

if (!status) // false
  console.log('status: false');
````

````
# 精要判斷式
status == true ? 'true' : 'false';
````

- switch ... case ...

````
# 標準寫法, default 敘述結束不需要寫 break 做結尾.
switch (status) {
  case '1':
    console.log('one');
    break;

  case '2':
    console.log('two');
    break;

  default:
    console.log('other');
}
````

