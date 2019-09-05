# JS 中常用的类型判断

## JavaScript 具有 7 中内置数据类型

> 基本数据类型：Undefined Null Boolean String Number;
> 引用数据类型：Object Symbol

## 常用的判断数据类型的方法：

- typeof
- instanceof
- Object.prototype.toString
- constructor

## 使用 typeof 判断类型

### 基本类型可以使用 typeof 来判断

> - typeof 5 //"number"
> - typeof 'aa' //"string"
> - typeof undefined //"undefined"
> - typeof true //"boolean"

#### typeof 判断 null 时显示 object ，null 是一个例外

#### 使用 typeof 判断 数组[]，日期 Date()，对象{}时显示“object"，判断函数 function 显示”function“,判断 Symbol 显示”symbol“

> 结论：使用 typeof 可以判断出除 null 以外的基本类型，以及 function 类型和 symbol 类型；null 会被 typeof 判断为 object

## 使用 instanceof 判断类型

> 用来判断创建的对象是否是构造函数的实例

## 使用 constructor 和 Object.prototype.toString 判断类型

#### 使用 Object.prototype.toString 判断类型

> - Object.prototype.toString.call(1) [Obejct Number]
> - Object.prototype.toString.call("aa") [Obejct String]
> - Object.prototype.toString.call(true) [Obejct Boolean]
> - Object.prototype.toString.call(undefined) [Obejct Undefined]
> - Object.prototype.toString.call(null) [Obejct Null]
> - ....

#### 使用 constructor 可以查看目标的构造函数。对应 undefined 和 null 如果尝试读取 constructor 属性会报错
