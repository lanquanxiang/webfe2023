# 0. 工程素养
1. 需要注意开发细节问题，注意测试
2. 应该多学一些解决方案，根据实际情况来进行选择

# 1. 列表
1. 有序列表
	1. 标记 ol>li
	2. 属性 type="1 | A | a | I | i"
2. 无序列表
	1. 标记 ul>li
	2. 属性 type="disc | circle | square | none"
3. 定义列表
	1. 标记 dl dt dd
4. 嵌套列表
	1. ul>li>ul>li
	2. 有序+无序
	3. 注意：二级列表需要正确嵌套，嵌入到li的文本中
	
# 2. 图像
1. 标记及属性 img src alt title width height
2. 路径的编写(重点)
	扩展：
	1. 路径有哪几种？
	2. 这些路径有什么优缺点？-->选择

# 3. 超链接
1. 标记及重要属性 a href target="_blank | 自定义的框架名称"
2. 应用：
	1. 常规链接  target  
	2. 书签链接
		1. 作用？什么时候用？
		2. 怎么做书签？
	3. 图像链接
	4. 其他（了解）：空白链接、邮件链接、区域链接、JS链接...
		1. href="" ==F5
		2. href="#" #top回到顶部
		3. href="javascript:void(0);" 自定义行为，需要JS辅助

# 4. 表格
1. 表格标记（掌握）及常用属性（了解）
2. 表格单元格的合并（掌握）
	rowspan colspan
3. 表格结构标记（了解）
	1. thead tbody  tfoot
	2. 在tr外面加一个壳子，方便对多行进行统一操作    table>tr>td   table>thead>tr>td