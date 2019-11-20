# ES5 正規化

## 正規化取代

````
var text = "Hello, I am Leonardo, I love the greatest artist Leonardo Da Vinci, And the famous actor Leonardo Dicaprio.";

# 僅取代第一個出現的位置
text.replace("Leonardo", "Michelangelo"); // Hello, I am Michelangelo, I love the greatest artist Leonardo Da Vinci, And the famous actor Leonardo Dicaprio.

# 正規化取代文字
text.replace(/Leonardo/g, "Michelangelo"); // Hello, I am Michelangelo, I love the greatest artist Michelangelo Da Vinci, And the famous actor Michelangelo Dicaprio.

# 正規化取代文字(大小寫不敏感)
text.replace(/leonardo/ig, "Michelangelo"); // Hello, I am Michelangelo, I love the greatest artist Michelangelo Da Vinci, And the famous actor Michelangelo Dicaprio.
````

## test
__正規化測試是否出現於字串__

````
var text = "Hello, I am Leonardo, I love the greatest artist Leonardo Da Vinci, And the famous actor Leonardo Dicaprio.";

var pattern = new RegExp("Leonardo");
pattern.test(text); // true
````

## match
__回傳符合正規化文字(陣列方式)__

````
var text = "Hello, \nI am Leonardo, \nI love the greatest artist Leonardo Da Vinci, \nAnd the famous actor Leonardo Dicaprio.";

# m 換行處之後是否符合該正規化文字
text.match(/^I/gm); // ['I', 'I'];
````