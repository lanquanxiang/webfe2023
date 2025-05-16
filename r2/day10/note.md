# 1. 节点操作
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