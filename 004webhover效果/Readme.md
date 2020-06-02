# web hover效果
[web hover效果 油管搬运](https://www.bilibili.com/video/BV1dc411h76P)

## 知识点
- [ ] box-shadow
- [ ] css动画
- [ ] nth-child

---

### box-show
box-shadow属性可以设置一个或多个下拉阴影的框。

#### 语法
    box-shadow: h-shadow v-shadow blur spread color inset;
> 注意：boxShadow 属性把一个或多个下拉阴影添加到框上。该属性是一个用逗号分隔阴影的列表，每个阴影由 2-4 个长度值、一个可选的颜色值和一个可选的 inset 关键字来规定。省略长度的值是 0。

|值|说明|
|:---|:---|
|h-shadow|必需的。水平阴影的位置。允许负值|
|v-shadow|必需的。垂直阴影的位置。允许负值|
|blur|可选。模糊距离|
|spread|可选。阴影的大小|
|color|可选。阴影的颜色。在CSS颜色值寻找颜色值的完整列表|
|inset|可选。从外层的阴影（开始时）改变阴影内侧阴影|

[CSS3 box-shadow 属性](https://www.runoob.com/cssref/css3-pr-box-shadow.html)

### css动画
1. 动画是使元素从一种样式逐渐变化为另一种样式的效果。
2. 您可以改变任意多的样式任意多的次数。
3. 请用百分比来规定变化发生的时间，或用关键词 "from" 和 "to"，等同于 0% 和 100%。
> 0% 是动画的开始，100% 是动画的完成。
> 为了得到最佳的浏览器支持，您应该始终定义 0% 和 100% 选择器。

[CSS3动画是什么？](https://www.runoob.com/css3/css3-animations.html)


### nth-child
:nth-child(n) 选择器匹配属于其父元素的第 N 个子元素，不论元素的类型。

**n 可以是数字、关键词或公式。**
1. 直接写上数字，表示第几个第几个
2. Odd是奇数，even是偶数（第一个子元素的下标是 1）。
3. 使用公式 (an + b)。描述：a 表示周期的长度，n 是计数器（从 0 开始），b 是偏移值。

[CSS3 :nth-child() 选择器](https://www.w3school.com.cn/cssref/selector_nth-child.asp)