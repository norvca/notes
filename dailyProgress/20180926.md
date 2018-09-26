# 一句话系列

### 1. javascript 里一切引用类型皆对象
所以得除去 string、number、boolean、null、udefined 等值类型

### 2. javascript 里所有对象都是实例化而来的 
```js
var baz = { name: 'bob' }
// 相当于
var baz = new Object();
baz.name = "bob";

function foo() {};
// 相当于
var foo = new Function();
```

### 3. `__proto__ ` 是对象实例化时产生的， `__proto__` 总是指向类的 prototype 属性
```js
var date = new Date();
date.__proto__ === Date.prototype; // true
```

### 4. 对象都包含`__proto__`属性，只有类才包含 prototype 属性。

```js
var date = new Date();
date.prototype // undefined
// Date 本身也是对象，的所以 Date 包含 __proto__ 属性
```



