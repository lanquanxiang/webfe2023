# 1. Ajax概念（异步的JavaScript 和 XML）
1. 作用：在不刷新页面的情况下，更新页面内容（向服务器发起请求）
2. 优点（理解、简答题）：
	1. 异步：提高效率，不影响用户的其他操作；扩展：也可以发起同步请求（什么时候用？）
	2. 按需更新：使用JS来控制页面内容（获得的数据显示在需要的位置）
		扩展：节省带宽、减轻浏览器渲染的压力...
	3. 数据和显示分离：数据存储在txt、xml、json（重点：前后端分离开发）
3. 缺点（了解）：
	1. 安全问题： 扩展（AI）：什么是跨域请求？如何解决跨域的问题？
	2. 开发维护问题：不便于处理复杂的错误，不便于调试
	3. 搜索问题：URL不变化，内容在变，对搜索引擎、网址收藏都不友好

# 2. Ajax的应用
## 1. 请求文本数据
1. 同步请求文本数据
	1. 创建核心对象
	2. 创建请求
	3. 发送请求
	4. 接收数据、显示
2. 异步请求文本数据
	1. 请求状态发生改变触发事件
	2. 请求状态==4
	3. 服务状态==200
## 2. 请求XML数据
1. 如何编写XML
2. 如何解析XML数据
## 3. 请求JSON数据
1. 如何编写JSON
2. 如何解析JSON

	
	