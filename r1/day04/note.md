# 0. 工程素养
1. 可维护性和可扩展性：CSS将内容和显示分离
2. 团队协作：慎用id选择器、style行内样式、important

# 1. CSS
1. CSS概念以及特点（了解）
	1. 层叠样式表
	2. 装饰网页
	3. 让显示和内容分离-->分工合作-->可维护性、可读性、渲染效率
	4. 特性：继承、层叠（样式叠加、覆盖）
2. CSS语法： 选择器{声明；声明；声明；...}【掌握】
	1. 怎么写？
	2. 注意事项
3. CSS的使用
	1. 外链式
		1. 创建css文件
		2. link标签链接文件，href指定路径
	2. 导入式
		1. 创建css文件
		2. style标签中使用@import导入css文件，url()函数来指定路径
	3. 内部样式
		1. 直接在网页中（head标签）使用style标签
		2. 在style标签中直接书写css
	4. 行内样式
		1. 直接在元素的标签中使用style属性
		2. 在style属性的值中书写css
	扩展：上面不同写法的优缺点。
		1. 方法1和方法2的区别？ 加载时间不一样、兼容性不一样
		2. 方法1/3/4的适用场景。
4. CSS的选择器
	
5. 选择器的优先级
	1. 外部样式、内部样式（从上到下，后面的样式会覆盖前面的样式）
	2. 行内样式优先级>外部、内部

# 2. CSS的选择器
## 1. 常用选择器
1. 通配符选择器 * ：设置默认样式、清除浏览器默认样式
2. id选择器
3. class选择器
4. 元素选择器
## 2. 组合选择器
1. 后代选择器 E F 选中F，F是E的后代
2. 父子选择器 E>F 选中F，F是E的儿子
3. 相邻兄弟选择器 E+F 选中F，F是E的相邻兄弟
4. 普通兄弟选择器 E~F 选中F，F是E的兄弟（后驱）
5. 群组选择器 E,F 选中E或F
## 3. 属性选择器
1. [attribute=value]
2. [attribute^=value]
3. [attribute$=value]
4. [attribute*=value]
## 4. 伪元素（虚拟元素）选择器
1. ::before
2. ::after
3. 属性：content:"文本"  content:url()
## 5. 伪类（特殊状态）选择器
1. :hover
2. :empty
3. E:nth-child(x) x的取值：数字、表达式An+b、关键词（odd、even）
扩展：链接伪类（选择器需要遵守书写顺序“爱恨原则”）

## 6. 选择器优先级
1. 能够计算/判断不同选择器的优先级
2. 在开发过程中有意识的控制选择器的优先级
