# 0. 工程素养
1. 能够使用js实现无条件的页面跳转，禁止不经过用户同意，强制跳转到非法网页
2. 能够使用js打开新的窗口，禁止无限制的打开窗口（浏览器有限制）

# 1. DOM（节点）操作
## 1. 节点（了解）
1. 文档树中有哪些类型的节点？
2. 节点之间的关系以及如何获取？【属性】
## 2. 节点的操作
1. 增
	1. 创建元素createElement
	2. 修改元素（修改文本、修改属性）
	3. 将元素加入网页appendChild
	注意：使用appendChild追加节点，文档树刷新，页面重新渲染。如果大量追加节点，效率降低
	扩展：批量追加节点（文档碎片）
		1. 如何创建文档碎片
		2. 将节点加入碎片中
		3. 将碎片加入网页中
2. 删
	1. removeChild
	2. 删除第一个孩子、删除最后一个孩子
	扩展：节点的克隆clone、节点的替换replace
3. 改（4-3-5 修改文本、属性、样式）
4. 查（4-3-2 6种方法）

# 2. BOM(window)
## 1. 如何实现网页跳转？
1. location.href（读，写--跳转）
## 2. 如何实现打开和关闭窗口？
1. let w_id = open(url,name,特征)
2. w_id.close()
## 3. 如何实现交互提示框（警告、确认、询问框）
1. alert()
2. confirm()
3. prompt()
## 4. 网页定时器
1. 如何设置定时器（一次性、周期性）
2. 如何清除定时器
扩展：【面试】JS事件轮询、JS事件执行过程
## 5. 其他（浏览记录、前进、后退、cookie）
