#### 待确认问题
1. 内联格式化上下文
2. 可继承的样式属性
3. 内联盒子模型
4. font-family 和 font-size 怎么影响基线

#### 如何解决问题
块状元素里的行内元素如何垂直居中，行内元素里包括text文本，img图片等
行内元素设置vertical-align: middle
碰到其他诡异问题（考虑vertical-align，line-height, font-size, 还有幽灵空白元素）
行内元素设置宽高没有用，行内元素由其内的元素决定宽高（auto*auto）

#### 概念区分 (inline-box（行内框）、line-box（行框/行盒）、containing（包含） box 和 content area（内容区域）))

#### 基线确定方式

1. 行内元素，块状元素内部，inline-block元素内部（默认存在幽灵空白节点，相当于一个x在内部，基线也基于x的下边缘）
2. inline-block元素，如果里面没有inline内联元素，或者overflow不是visible，则该元素的基线就是其margin底边缘，否则，其基线就是元素里面最后一行内联元素的基线。