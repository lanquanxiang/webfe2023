# 1. 对元素的操作（增删改查）
1. 查询 $(选择器)
	1. $(CSS选择器)
	2. $(选择器:first)  $(选择器:eq(index))  位置选择器
	3. $(:text) $(:disabled) 筛选器
	4. 常用方法 $(选择器).eq(index)  $(选择器).get(index)  $(选择器)[index]
2. 修改
	1. 修改文本 jQuery对象.html() jQuery对象.text()
	2. 修改标签的属性 jQuery对象.attr("src") jQuery对象.attr("src","新地址")
	3. 修改值（特殊的对象属性） jQuery对象.val() == jQuery对象.prop("value")
	4. 修改对象的属性   jQuery对象.prop()
	5. 修改样式
			1. DOM对象--- 设置style属性，间接控制CSS样式
			2. jQuery对象--- 对象.css(样式)    对象.addClass(class的名字)
3. 增加
4. 删除