# 1. jQuery
## 1. 概念
1. jQuery是JS的库（引入 *.js）
2. jQuery作用：简化操作
## 2. jQuery引入
1. 下载jQuery到本地，然后通过script引入
2. 直接通过script引入网络资源

# 2. 如何使用jQuery来实现事件响应
## 1. 事件响应【掌握】
1. 通过jQuery对象直接触发特定事件   ```$("button").click(function(){})```
2. 为jQuery对象绑定特定事件  ```$("button").bind/unbind/one("click",function(){})```
3. 为jQuery对象绑定特定事件(动态)  ```$("button").on/off("click",function(){})```
## 2. 模拟用户操作
```
setInterval(function(){
$("#barragetext").val("666")
$("#sendbarrage").click()
},1000)
```
## 3. 链式语法（简化代码：AI）
## 4. jQuery事件
1. 类似DOM事件
2. 特殊 ready事件【重点】 
	1. ready事件和onload事件的区别？【重点】
	2. 如何在网页中使用ready 		```$(function(){ .... .... })```

# 3. 如何使用jQuery来实现节点操作
1. 增加
2. 删除
3. 修改
	1. 修改文本
		DOM方法：innerHTML、innerText、textContent
		jQuery：html("<b>新文本</b>")、text("新文本")
	2. 修改HTML的属性
		1. attr()
	3. 修改对象的属性
		1. 获取值 val()   prop("value")
		2. 获取其他值 prop()
		扩展： is() not()		
	4. 修改样式
		setAttribute("style","color:red;font-zise:16px;") 
		//编写复杂，不方便维护，覆盖原来的行内样式
		1. 获取单条样式的值  css("样式的名称")
		2. 设置单条样式的值   css("样式的名称",值)
		3. 设置多条样式的值  css(JSON串)
		4. 设置/移除多条样式  addClass/removeClass(类名)  需要在外部提前定义此类的样式
		
4. 查询（获得）
	1. 创建新的jQuery对象    $("<img/>")
	2. 将DOM对象转换为jQuery对象：希望使用jQuery的方法   $(DOM对象)
	3. 获取网页上已经存在的元素   
		1. $("选择器")
		2. $("选择器:位置")
		3. $(":筛选选择器")
		4. $("选择器").eq(索引)   $("选择器").get(索引) $("选择器")[索引]
		5. 扩展：jQuery对象和DOM对象相互转换
			1. jQuery对象变为DOM对象：  jQuery对象[0]
			2. DOM对象变为jQuery对象：  $(DOM对象)