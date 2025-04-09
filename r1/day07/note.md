1. HTML：标识内容（标记）
2. CSS：装饰内容（选择器、样式）
3. JavaScript（JS）：控制内容（事件+增删改查）
# 0. 工程素养
1. 不开发恶意脚本
2. 防御性编程
# 1. JavaScript基础知识
1. JS的构成？ JS语法+DOM+BOM
2. JS的作用？
3. JS的使用？

# 2. JS的基本语法
1. 变量的声明 var或let、const（比较少）  扩展：他们的区别？
2. 变量声明的提升（重要【面试】）

# 3.函数（function、Object）
1. 函数的定义
	1. function关键字定义函数
	2. var fun = 函数表达式
2. 函数的调用

# 4. 常用对象
## 1. 元素(Element)【重要】
1. 获得element[重要] 注意索引（id和querySelector）
2. 修改
	1. 获取/修改内容 innerHTML/innerText
	2. 增删改查属性 x.id x.class x.value
		· x.addAttribute("属性","属性值")
		· x.removeAttribute("属性")
		· x.setAttribute("属性","属性值")
		· x.getAttribute("属性")
### 数字
1. 以0开头的数字是八进制 010+100+001=109
2. 以0x开头的数字是十六进制
3. 浮点数整数部分为0可以省略 .1+.2=？
4. 如何判断两个浮点数相等？ if(a==b)??? if(abs(a-b)<1e-15)
5. [面试]0.1+0.2=？ 0.300...00004 为什么不是0.3？怎么让他等于0.3？（调整精度）
6. Infinity无穷大？-Infinity   
	1. 什么时候出现？ 1/0
	2. 如何判断？ isFinite()
7. NaN （Not a Number） typeof判断类型
	1. 什么时候出现？ 0/0 
	2. 如何判断？ isNaN() 校验表单中是否是数字（类型转换：字符串转换为数字）
	3. NaN和任何值进行算术运算都是NaN
	4. NaN和任何值进行逻辑运算都是false
	5. NaN和任何值都不相等，包括NaN
### 运算和类型转换
1. "+" 如果操作数两端，任意一端是字符串，字符串拼接
2. "-" 首先会将操作数两端转换为数字，在运算，不能转换变为NaN
3. "==" 只判断值，如果操作数两端类型不相同，进行转换之后再比较【扩展，面试】
4. "===" 判断类型和值（建议）
### 类型转换
1. 转数字
	1. Number(xxx) NaN  "11true"
	2. parseInt(xxx)/parseFloat(xxx) 解析  "1.1true"==11  "true11" NaN
	3. -0  *1  /1  
2. 转字符串
	1. String()
	2. xxx.toString()  xxx不能是异常对象
	3. +""
3. 转布尔 Boolean(xxx)  0、-0、null、false、NaN、undefined，或空字符串
### 任务
1. 完善计算器的加法
2. 解决0.1+0.2
3. 判断输入的是不是数字？如果不是数字，中断函数 return;
4. 考虑优化代码（重复太多了）