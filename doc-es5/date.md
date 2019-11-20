# ES5 日期方法

## getFullYear
__取得年份__

````
var date = new Date();
date.getFullYear(); // 2018年
````

## getMonth
__取得月份(0-11)__

````
var date = new Date();
date.getMonth(); // 11月(10)
````

## getDate
__取得日期(1-31)__

````
var date = new Date();
date.getDate(); // 28日
````

## getHours
__取得小時(0-23)__

````
var date = new Date();
date.getHours(); // 早上12點(0)
````

## getMinutes
__取得分鐘(0-59)__

````
var date = new Date();
date.getMinutes(); // 40分
````

## getSeconds
__取得秒鐘(0-59)__

````
var date = new Date();
date.getSeconds(); // 40秒
````

## getDay
__取得週幾(0-6)__
-----

````
var date = new Date();
date.getDay(); // 週3
````

----

## setFullYear
__設定年份__

````
var date = new Date();
date.setFullYear(2020); // 2020年
````

## setMonth
__設定月份(0-11)__

````
var date = new Date();
date.setMonth(11); // 12月
````

## setDate
__設定日期(1-31)__

````
var date = new Date();
date.setDate(25); // 25日
````

## setHours
__設定小時(0-23)__

````
var date = new Date();
date.setHours(11); // 早上11點
````

## setMinutes
__設定分鐘(0-59)__

````
var date = new Date();
date.setMinutes(59); // 59分
````

## setSeconds
__設定秒鐘(0-59)__

````
var date = new Date();
date.setMinutes(59); // 59分
````
-----

## getUTCFullYear
__取得 UTC 時間(+0)年份__

````
var date = new Date();
date.getUTCFullYear(); // 2018年
````

## getUTCMonth
__取得 UTC 時間(+0)月份(0-11)__

````
var date = new Date();
date.getUTCMonth(); // 11月(10)
````

## getUTCDate
__取得 UTC 時間(+0)日期(1-31)__

````
var date = new Date();
date.getUTCDate(); // 28日
````

## getUTCHours
__取得 UTC 時間(+0)小時(0-23)__

````
var date = new Date();
date.getUTCHours(); // 下午4點(16)
````

## getUTCMinutes
__取得 UTC 時間(+0)分鐘(0-59)__

````
var date = new Date();
date.getUTCMinutes(); // 40分
````

## getUTCSeconds
__取得 UTC 時間(+0)秒鐘(0-59)__

````
var date = new Date();
date.getUTCSeconds(); // 40秒
````

## getUTCDay
__取得 UTC 時間(+0)週幾(0-6)__

````
var date = new Date();
date.getUTCDay(); // 週2
````

-----

## setUTCFullYear
__設定 UTC 時間(+0)年份__

````
var date = new Date();
date.setUTCFullYear(2020); // 2020年
````

## setUTCMonth
__設定 UTC 時間(+0)月份(0-11)__

````
var date = new Date();
date.setUTCMonth(); // 12月(11)
````

## setUTCDate
__設定 UTC 時間(+0)日期(1-31)__

````
var date = new Date();
date.setUTCDate(25); // 25日
````

## setUTCHours
__設定 UTC 時間(+0)小時(0-23)__

````
var date = new Date();
date.setUTCHours(3); // 上午3點(3)
````

## setUTCMinutes
__設定 UTC 時間(+0)分鐘(0-59)__

````
var date = new Date();
date.setUTCMinutes(59); // 59分
````

## setUTCSeconds
__設定 UTC 時間(+0)秒鐘(0-59)__

````
var date = new Date();
date.setUTCSeconds(59); // 59秒
````
-----

## now
__取得現在時間戳記__

````
Date.now(); // 1543496642827
````

## parse
__將文字轉換成時間戳記__

````
Date.parse('November 24,2018'); // 1542988800000
````

## UTC
__輸入 UTC 時間(+0)轉換成時間戳記__

````
Date.UTC(2018, 11, 24); // 1545609600000
````

## getTime
__取得現在時間戳記__

````
var date = new Date();
date.getTime(); // 1545609600000
````

## setTime
__設定現在時間戳記__

````
var date = new Date();
date.setTime(1545609600000); // Mon Dec 24 2018 08:00:00 GMT+0800 (台北標準時間)
````
## getTimezoneOffset

````
var date = new Date();
date.getTimezoneOffset(); // -480
````

-----

## toTimeString
__取得時間__

````
var date = new Date();
date.toTimeString(); // 22:55:55 GMT+0800 (台北標準時間)
````

## toDateString
__取得日期__

````
var date = new Date();
date.toDateString(); // Fri Nov 30 2018
````

## toString
__取得時間日期__

````
var date = new Date();
date.toString(); // Thu Nov 30 2018 20:55:55 GMT+0800 (台北標準時間)
````

## toISOString
__取得 Zulu 時間日期(+0)__

````
var date = new Date();
date.toISOString(); // 2018-11-30T23:55:55.099Z
````

## toLocaleString
__取得本機時間日期__

````
var date = new Date();
date.toLocaleString(); // 2018/11/29 下午10:39:37
````

## toUTCString
__取得 UTC 時間日期(+0)__

````
var date = new Date();
date.toUTCString(); // Fri, 30 Nov 2018 12:55:55 GMT
````
