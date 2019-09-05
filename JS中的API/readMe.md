# JavaScript 中的 API

## 用原生 js 实现 jq 的 offset 方法

> - 通过递归实现
> - 通过 getBoundingClientRect 实现

- [通过递归实现](Demo_1.html)
- [通过 getBoundingClientRect 实现](Demo_2.html)

## 数组 reduce 方法的相关实现

> 语法：arr.reduce(function(previousValue,currentValue,currentIndex,array)[,initialValue])

- reduce 第一个参数 callback 是核心，它对数组的每一项进行“叠加加工”，其最后一次返回的值作为 reduce 方法的最终返回值。它包含四个参数
- previousValue：表示“上一次”callback 函数的返回值
- currentValue：数组遍历中正在处理的元素
- currentIndex：可选，表示 currentValue 在数组中对应的索引，如果提供了 initialValue，则索引为 0，否则为 1；
- array：可选，调用 reduce 的数组；
- initialValue：可选，作为第一次调用 callback 时的第一个参数，如果没有提供 initialValue，那么数组中的第一个元素将作为 callback 的第一个参数

### 练习

> - [数组 reduce 方法的使用](Demo_3.html)
> - [实现一个 reduce](Demo_4.html)
