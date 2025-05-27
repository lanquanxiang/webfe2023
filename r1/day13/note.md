# jQuery
1. JS库 *.js（引入库之后，可以简化JS操作）
2. 如何简化操作？（使用jQuery来处理事件响应，怎么来控制网页元素）

# 1. jQuery的导入
1. 本地导入
2. 在线导入

# 2. jQuery对象获取
1. 创建对象 $(DOM对象)  $(网页元素) 【掌握】
2. 获取已经存在的对象
	1. $(选择器)  【掌握】
	2. 位置选择器
	3. 筛选器
3. 通过jQuery方法来获取
	1. $("selector").eq(index)			//jQuery对象
	2. $("selector").get(index)		//DOM对象
	3. $("selector")[index]			//DOM对象
	4. 扩展：DOM对象可以和jQuery对象相互转换

# 3. jQuery的事件响应
1. jQuery触发事件 $(选择器).click(函数)
2. 【了解，开发（脚本）】模拟用户操作
```
$("#barragetext").val("666")
$("#sendbarrage").click()
```
3. [重要]事件绑定
	1. jQuery对象.one("事件","函数")
	2. jQuery对象.bind("事件","函数")
	3. jQuery对象.unbind("事件","函数")
	4. jQuery对象.on("事件","函数")
	5. jQuery对象.off("事件","函数")
## 总结：事件响应
1. 直接在标签中添加事件响应
2. 获得DOM元素，为事件属性赋值
3. 获得DOM元素，为元素添加事件监听【可以移除事件监听】
4. $(选择器)获得jQuery对象，jQuery对象.click(函数)
5. $(选择器)获得jQuery对象，jQuery对象.bind("事件","函数")
6. $(选择器)获得jQuery对象，jQuery对象.on("事件","函数")

# 4. 对元素的操作（增删改查）
1. 查询 $(选择器)
2. 修改
	1. 修改文本 jQuery对象.html() jQuery对象.text()
	2. 修改HTML属性 jQuery对象.attr("src") jQuery对象.attr("src","新地址")
	3. 修改值 jQuery对象.val()
	4. 修改DOM对象的属性   jQuery对象.prop()
3. 增加
4. 删除

