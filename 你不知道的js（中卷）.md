第一章：类型
1.2
内置类型：
空值（null）、未定义（undefined）、布尔值（boolean）
数字（number）、字符串（string）、对象（object）
符号（symbol,ES6新增）
特殊：typeof null==="object";
null是基本类型中唯一一个假值，typeof对它的返回值是“object”
在函数中，函数对象的length属性是其声明的参数的个数
在数组中，其length属性是元素的个数
1.3
js中变量是没有类型的，只有值才有。
注意：typeof运算符总是会返回一个字符串
undefined和undeclared：
已在作用域中声明但还没有赋值的变量是undefined
还没有在作用域中声明过的变量是undeclared
可以通过typeof的防范机制来检查undeclared变量


第二章：值
2.1数组
js中的数组可以容纳任何类型的值
类数组：一组通过数字索引的值
2.2字符串
js中字符串是不可变的，而数组是可变的
字符串不可变是指字符串的成员函数不会改变其原始值
字符串怎样实现倒转：
先将字符串转换为数组，待处理完后再将结果转换回字符串
2.3
js中整数和浮点数都是number类型
js中的数字常量一般用十进制表示，
不仅小数点后小数部分最后面的0可以省略，数字前面的0也可以省略
特别大和特别小的数字默认用指数格式显示，
与 toExponential() 函数的输出结果相同

tofixed(..) 方法可指定小数部分的显示位数
toPrecision(..) 方法用来指定有效数位的显示位数

42.tofixed(3) 是无效语法，因为 . 被视为常量 42. 的一部分
42..tofixed(3) 则没有问题
2.3.2较小的数值
对浮点数中的0.1+0.2不等于0.3，因为0.1 0.2并不是十分精确
2.3.4
ES6中的Number.isInteger(..) 方法可以检测一个值是否是整数
ES6中的Number.isSafeInteger(..)方法可以检测一个值是否是安全的整数
2.4
undefined和null
null 指空值（empty value）
undefined 指没有值（missing value）
或者：
undefined 指从未赋值
null 指曾赋过值，但是目前没有值
（undefined是标识符）
43页





