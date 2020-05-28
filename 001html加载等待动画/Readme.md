# 知识点

- [ ] meta中viewport的含义
- [ ] svg的用法
- [ ] circle的用法
- [ ] box-sizing
- [ ] stroke-dasharray、stroke-dashoffset
- [ ] transform-origin、transform
- [ ] animation动画相关

【转自B站】[html加载等待动画 安卓加载等待动画 svg 超级简单 新手入门](https://www.bilibili.com/video/BV1wt4y1y7dR)

-------

### meta中viewport的含义
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0,minimum-scale=1.0,user-scalable=0" />


|属性名|备注|
|:---|:---|
|width|设置layout viewport 的宽度，为一个正整数，使用字符串”width-device”表示设备宽度|
|initial-scale|设置页面的初始缩放值，为一个数字，可以带小数 
||minimum-scale|允许用户的最小缩放值，为一个数字，可以带小数|
|maximum-scale|允许用户的最大缩放值，为一个数字，可以带小数|
height|设置layout viewport 的高度，这个属性对我们并不重要，很少使用|
|user-scalable|是否允许用户进行缩放，值为”no”或”yes”, no 代表不允许，yes代表允许|


### stroke-dasharray、stroke-dashoffset
1. **stroke意思是：画短线于，在...上划线**
2. **stroke-dasharray: 用于创建虚线，之所以后面跟的是array的，是因为值其实是数组。请看下面解释**

> stroke-dasharray = '10'
> stroke-dasharray = '10, 5'
> stroke-dasharray = '20, 10, 5'
 
stroke-dasharray为一个参数时： 其实是表示虚线长度和每段虚线之间的间距
　　如：stroke-dasharray = '10' 表示：虚线长10，间距10，然后重复 虚线长10，间距10两个参数或者多个参数时：一个表示长度，一个表示间距
　　如：stroke-dasharray = '10, 5' 表示：虚线长10，间距5，然后重复 虚线长10，间距5
　　如：stroke-dasharray = '20, 10, 5' 表示：虚线长20，间距10，虚线长5，接着是间距20，虚线10，间距5，之后开始如此循环

 

3. **stroke-dashoffset： offset：偏移的意思。**
这个属性是相对于起始点的偏移，正数偏移x值的时候，相当于往左移动了x个长度单位，负数偏移x的时候，相当于往右移动了x个长度单位。
需要注意的是，不管偏移的方向是哪边，要记得dasharray 是循环的，也就是 虚线-间隔-虚线-间隔。
这个属性要搭配stroke-dashoffset才能看得出来效果，非虚线的话，是无法看出偏移的。

[SVG学习之stroke-dasharray 和 stroke-dashoffset 详解](https://www.cnblogs.com/daisygogogo/p/11044353.html)


### box-sizing
box-sizing 属性允许您以特定的方式定义匹配某个区域的特定元素。

例如，假如您需要并排放置两个带边框的框，可通过将 box-sizing 设置为 "border-box"。这可令浏览器呈现出带有指定宽度和高度的框，并把边框和内边距放入框中。

[CSS3 box-sizing 属性](https://www.w3school.com.cn/cssref/pr_box-sizing.asp)


### transform-origin、transform
transform-origin 属性允许您改变被转换元素的位置, 设置旋转元素的基点位置
2D 转换元素能够改变元素 x 和 y 轴。3D 转换元素还能改变其 Z 轴。
> 注释：该属性必须与 transform 属性一同使用。

[CSS3 transform-origin 属性](https://www.w3school.com.cn/cssref/pr_transform-origin.asp)


### animation动画相关
需要先使用 @keyframes 规则创建以后的新样式。
然后将动画绑定到选择器：规定动画的名称，规定动画的时长

[CSS3 动画](https://www.w3school.com.cn/css3/css3_animation.asp)