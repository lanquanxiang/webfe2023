# jQuery
1. JavaScript的库（*.js）
2. 使用jQuery可以简化DOM操作
# 1. jQuery的导入
1. 下载（在线文档）
2. 引入外部脚本
# 2. jQuery对象
1. 直接创建  $(元素)
2. 将已经存在的DOM对象转换为jQuery对象  $(DOM对象)
3. 获取已经存在的网页元素  $(选择器)
# 3. 使用jQuery实现事件响应
1. jQuery元素.事件(函数)   btn.click(fun)
	1. 扩展：模拟用户操作
	```
	setInterval(function(){
		$("#barragetext").val("666");
		$("#sendbarrage").click();
	},2000)
	```
	2. jQuery特有事件：ready（加载文档树之后执行） = load(所有资源和数据加载完毕之后执行)
	```
	$(document).ready(function(){  网页加载之后的代码   })
	```
2. jQuery事件绑定 jQuery元素.bind/unbind/one("事件","函数")  【静态】
3. jQuery事件绑定 jQuery元素.on/off("事件","函数")  【动态】

# 4. 使用jQuery来对DOM元素进行增删改查
1. 查询：选择器、位置选择器、筛选器、索引函数
2. 修改：
	1. 文本  text()/html()
	2. 属性（标签属性、对象属性）
	3. 样式