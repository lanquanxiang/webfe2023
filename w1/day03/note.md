# 0. 工程素养
1. 保障用户数据安全，敏感数据采用post
2. 保障数据一致性，单选、多选、下拉列表，给用户看的内容==传输给服务器
3. 提高用户体验，控件分组、扩大焦点。。。
4. 保障系统安全，disabled禁用数据，如学号，银行账号
5. 只有最合适的，没有最好的

# 1. 表单（重点，考试第一个编程题）
1. 作用？收集数据
2. 语法？
	```
		<form action="处理数据的网址" method="get|post" enctype="MIME">
			
		</form>
	```
	扩展：MIME（标识资源类型） 一级媒体类型/二级类型
		text 文本
		video 视频
		audio 音频
		image 图像  image/jpg
		application 应用
		message 信息
		multipart 多部分媒体
	扩展：get和post的区别？（问答，面试）
3. 构成：
	1. 输入控件（重点）

# 2. 输入控件
1. 语法
	```
		<input type="HTML4.01中有10个类型" name="参数的名字" value="值"/>
	```
2. 输入控件的类型
	1. 四个框： text/password/radio/checkbox
	2. 四个按钮：button/submit/reset/image
	3. 两个域：hidden/file
3. 注意事项
	1. 如果控件没有name属性，此控件无效（没有作用了）
	2. 按钮的value属性表示的是按钮上的文字
	3. 其他控件的value属性表示的是参数的默认值
	4. 同一组单选按钮需要设置相同的名字
	5. 如果是鼠标直接点击或选择的控件（单选、多选），必须设置value
	6. 多选框，建议设置相同的名字，方便服务器端批量接受数据
	7. 如果表单中出现文件域，必须设置method为post，必须设置enctype
	8. 隐藏域必须设置name和value，用来传输默认参数
4. 属性
	1. checked，主要此属性存在，无论什么取值，都是默认选中
	2. disabled 使控件不可用，控件变成灰色，不能修改，信息不发送给服务器（hidden传输默认信息）
	3. readonly 使控件不可修改，控件没有变化，不能修改，信息回发给服务器

# 3. 按钮button
1. 语法
2. type属性用来标识标题的按钮
3. 知道不同按钮的区别

# 4. select下拉列表
1. 语法
2. 为什么？ 单选、多选，选项太多的时候，不方便直接放在网页上 
3. 重要属性：单选、多选、分组
	1. 三个标签：select  option  optgroup+lable
	2. 三个属性：可多选、数量、默认选中

# 5. textarea多行文本
1. 语法
2. 为什么？ text文本框：单行，信息展示不完整
3. 重要属性

# 6. 了解fieldset和label标记
1. fieldset组合控件，提高用户体验
2. lable扩大了获取焦点的范围，点击文字也可以输入内容

# 7. 页面框架（实验）
1. iframe
2. frameset