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
