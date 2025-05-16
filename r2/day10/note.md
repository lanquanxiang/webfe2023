# 0. 工程素养
1. 删除节点的时候：防御性编程，首先判断节点是否存在，防止异常
2. JS可以实现跳转：注意技术的边界，不能在他人的网上中嵌入无条件跳转代码，更不能跳转到非法网页
3. JS控制浏览器打开窗口：注意技术的边界，不能恶意的打开多个窗口

# 1. DOM节点操作
1. 增删 改（4-3-5）查（4-3-2）
2. 文档中节点的构成（节点树）
## 1. 增加节点
1. 创建元素document.createElement("标签");
2. 修改元素文本、属性
3. 追加到网页中（追加为最后一个孩子  / 追加到某个元素之前）
## 2. 批量增加节点
为什么：每增加一个节点都会重新渲染页面，如果增加太频繁，会降低渲染效率
1. 创建文档碎片document.createDocumentFragment()
2. 将节点加入碎片中
3. 将碎片加到网页中
扩展：前端优化策略（减少渲染次数）；AI:浏览器是如何渲染网页？
## 3. 删除节点
1. existingNode.removeChild(deleteNode)
2. deleteNode.parentNode.removeChild(deleteNode)
## 4. 节点克隆、节点的替换
1. var 新节点 = 旧节点.cloneNode(true); //深度克隆
2. 旧节点.parentNode.replaceChild(新节点, 旧节点);

# 2. BOM浏览器对象模型
## 1. window对象的常用属性
1. location：URL相关的信息
	1. location.href 可以实现网页跳转
2. window.document.cookie 信息存储（开发重要）
## 2. window对象的常用方法
1. 打开/关闭窗口
## 3. 交互框
1. 警告alert() 通知信息，不需要返回值
2. 确认confirm("确认信息?")
3. 询问