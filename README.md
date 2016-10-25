# flex
flex布局

2016年10月25日21:36:31

开篇发一下牢骚，最近一直在网投简历，居然一个面试机会都没有，可能是我简历写的不够漂亮，还是真的我能力有问题？可能我的知识体系是不够全面，毕竟是自学的嘛，

但我投的大部分都是小公司，他们要求都那么低，唉······，不知到该说啥

下面的笔记参考阮一峰老师博客写的

Flex是Flexible Box的缩写，意为"弹性布局"，用来为盒状模型提供最大的灵活性。

任何一个容器都可以指定为Flex布局。

设为Flex布局以后，子元素的float、clear和vertical-align属性将失效。
<h2>容器属性</h2>
```css
.box{
  display:flex;
}
```
行内元素使用flex
```css
.box{
  display:inline-flex;
}
```
Webkit内核的浏览器，必须加上-webkit前缀。
```css
.box{
  display:-webkit-flex;
  display:flex;
}
```
<h3>flex-direction</h3>
定义项目的排列方向
```css
.box{
  flex-direction:row | row-reverse | column | column-reverse;
}
```
它可能有4个值。

row（默认值）：从左到右

row-reverse：从右到左

column：从上到下

column-reverse：从下到时

<h3>flex-wrap属性</h3>
如果一条轴线排不下，如何换行。
```css
.box{
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```
nowrap（默认）：不换行。

wrap：换行，排在第一行在下方。

wrap-reverse：换行，排在第一行在上方。


<h3>flex-flow</h3>
flex-flow属性是flex-direction属性和flex-wrap属性的简写形式，默认值为row nowrap。
```css
.box {
  flex-flow: <flex-direction> || <flex-wrap>;
}
```
<h3> justify-content</h3>
justify-content属性定义了项目在主轴上的对齐方式。
```css
.box {
  justify-content: flex-start | flex-end | center | space-between | space-around;
}
```
flex-start（默认值）：左对齐

flex-end：右对齐

center： 居中

space-between：两端对齐，项目之间的间隔都相等。

space-around：每个项目两侧的间隔相等。所以，项目之间的间隔比项目与边框的间隔大一倍。

<h2>子节点属性</h2>
<h3>order属性</h3>
order属性定义项目的排列顺序。数值越小，排列越靠前，默认为0。
```css
.item {
  order: <integer>;
}
```

```css

```

```css

```

```css

```

```css

```

```css

```

```css

```

```css

```
