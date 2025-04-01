# 0. 工程素养
1. 浮动、特殊定位：脱离文档流，尽可能消除布局带来的影响
2. 用户体验：慎用fixed，永远固定在窗口中
# 1. CSS定位和布局
1. 元素位置：默认情况下，元素不能移动，在文档流中从上到下依次布局
2. 定位方式position
	1. relative：子绝父相；移动元素
	2. absolute：无论元素是否存在，都不影响网页布局
	3. fixed：是否不随滚动条滚动
3. 元素的浮动 float:left/right
	1. 脱离文档流
	2. 尽可能向上、尽可能向左向右
	应用：制作左右两侧菜单
	扩展（AI）：
		1. 浮动元素的特点
		2. 如何消除浮动带来的影响
		3. BFC布局
		4. 了解浮动的应用场景
# 2. CSS显示方式
1. overflow:新闻标题剪裁 hidden
2. visibility：hidden 不可见  == 完全透明（占用网页空间）
3. display：none 消失（不占用空间）
## display【重点】
1. block
2. inline-block
3. none
4. 课外：flex、grid 【重点】
# 3. CSS3新特性
1. border-radius:学会给盒子加圆角
2. border-image:用图像来做边框（知道图片如何分割）
3. box-shadow：类似text-shadow（实验）
4. filter：灰度滤镜
5. 变形和动画
	1. 定义简单动画
	2. 在关键帧设置2D变换（平移、拉伸、旋转）