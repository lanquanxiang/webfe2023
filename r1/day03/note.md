# 0. 工程素养
1. 保障用户信息安全，敏感数据需要post提交方式
2. 保障系统安全，禁止修改的数据考虑使用disabled + hidden
3. 保障业务安全，保障数据一致性，单选、多选、下拉列表控件给用户看的内容和传输给服务器的内容保持一致
4. 提高用户体验，下拉列表代替单选/多选（按需选择），考虑使用lable标签增加获得焦点的范围

# 1. 表单【重点（五颗星）】
1. 表单标记及重要属性
	1. 标记form
	2. 属性 action、method、enctype（文件上传的时候才会出现）
	扩展：
		1. get和post区别（考试问答，面试）
		2. MIME（多用途互联网邮件扩展类型：标识资源类型）
			1. text      text/html
			2. image     image/png
			3. audio
			4. video     video/mp4
			5. application
			6. message
			7. multiple 
2. 表单作用：收集数据 
3. 表单构成（重点）
	1. 输入控件
	2. 其他表单控件

# 2. input控件
1. 语法
2. input控件的多种类型
3. 开发中的注意事项
	1. 收集数据的控件必须设置name属性，否则此控件将被忽略，数据无法提交
	2. 单选框必须设置name属性，且同一组单选name的值必须相同
	3. 直接用鼠标点选的控件，必须要设置value，要和给用户的提示信息保持一致
	4. 多选框建议同一组设置为相同的名字，为了方便服务器接收数据
	5. 隐藏域必须设置name和value，用于传输默认值（不想让用户看见）
	6. 按钮（图像除外）的value用来设置按钮上的字，其他value用来设置默认值
	7. disabled属性让控件被禁用，变为灰色，不能获得焦点，不能修改，数据不能收集（hidden辅助）
	8. readonly属性让控件只读，外观不变化，不能获得焦点，不能修改，数据可以收集（用户体验不好）
	9. checked属性让选项被默认选中，只适用于单选、多选，无论取值。

# 3. button控件
1. 语法
2. 类型（三种）submit  reset  button
3. 区别
	1. 不同类型的区别 
	2. 和input中button的区别 == button类型

# 4. 下拉列表
1. 语法
2. 标记 select  option optgroup
3. 属性 multiple size selected

# 5. 多行文本
1. 语法
2. 重要属性 rows cols
3. 注意默认值（包含不可见字符）

# 6.  fieldset和label标记
1. 语法
2. 作用：提高用户体验

# 7. 页面框架（了解）
1. iframe
2. frameset