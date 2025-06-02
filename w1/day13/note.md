# jQuery
1. JavaScript库：*.js(文件) 
2. 为什么？"写得更少，做的更多" 简化了原来的操作（事件响应-->控制网页内容）
3. 下载jQuery，引入到网页中（引入外部脚本）

# 1. jQuery事件响应（对象、事件、函数）
1. jQuery对象.事件(函数)
2. jQuery对象.bind/unbind/one("事件",函数)
3. jQuery对象.on/off("事件",函数)  支持动态绑定

## 扩展知识
1. 模拟用户操作（脚本）
```
setInterval(function(){
	$("#barragetext").val("6")
	$("#sendbarrage").click()
},1000)
```
2. jQuery链式语法（AI）
3. 【重要】ready事件
   1. ready事件（网页文档树渲染成功，只需要标签加载完毕就可以了） 
   2. load事件（网页资源全部加载完毕，包括外部资源）
```
$(document).ready(function(){......})
$(function(){....} )
```

# 2. jQuery控制节点（增删改查）
## 1. 查询
1. 如何获得网页元素（jQuery对象）
	1. 创建新对象  $("<img/>")
	2. 将DOM对象转换为jQuery对象   $(DOM对象)
	3. 获取网页元素转为jQuery对象  $("选择器")
2. jQuery选择器
	1. 常规选择器 $("css选择器")
	2. 位置选择器
	3. 表单、状态筛选器
3. jQuery索引方法（从jQuery对象集合中找到自己想要的那一个）
	1. $("选择器").eq(索引)    --> jQuery对象
	2. $("选择器").get(索引)   --> DOM对象
	3. $("选择器")[索引]       --> DOM对象
	4. 扩展：jQuery对象和DOM对象相互转换
		1. DOM对象-->jQuery对象   $(DOM对象)
		2. jQuery对象-->DOM对象   jQuery对象[0]

## 2. 修改
1. 修改文本
	1. DOM对象：innerHTML、innerText、textContext
	2. jQuery对象: html()、text()
2. 修改标签属性
	1. DOM对象：set/getAttribute("属性"[,"值"])
	2. jQuery对象：attr("属性"[,"值"])
3. 修改对象属性(用户在网页中修改的内容)
	1. DOM对象：  对象.属性名   eg.  element.value
	2. jQuery：  对象.prop("属性名")  对象.val("值")
4. 修改样式
	1. DOM对象： 修改style属性，间接修改CSS
	2. jQuery对象： 对象.css(属性,属性值)  对象.css({CSS样式表})  对象.addClass(class名)
		
	