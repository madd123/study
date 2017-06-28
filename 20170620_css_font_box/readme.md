<!-- TOC -->

- [1. css font](#1-css-font)
    - [1.1. 字体](#11-字体)
        - [1.1.1. 标签默认样式](#111-标签默认样式)
        - [1.1.2. font](#112-font)
- [2. box 盒模型](#2-box-盒模型)
- [3. :before 和 :after伪类](#3-before-和-after伪类)
    - [3.1. margin-top bug](#31-margin-top-bug)
- [4. 作业](#4-作业)

<!-- /TOC -->
# 1. css font

## 1.1. 字体
### 1.1.1. 标签默认样式

p chrome 默认段前段后距离 1em,段前段后距离可以叠加

### 1.1.2. font

css原则1: css属性的展开写法，一定要写在缩写后面

```css
p{

    font-family:BiauKai,Microsoft YaHei,Arial;
    /*字体*/

    font-size:24px;
    /*文字大小*/

    line-height: 32px;
    /*行高*/

    font-weight:bold;
    /*b*/
    /*粗体*/
    /*400-900*/
    /*normal < 500 < bold*/

    font-style:italic;
    /*i*/
    /*斜体*/

    font: italic bold 16px/32px "微软雅黑";
    /*
        font-style
        font-weight
        font-size/line-height
        font-family
    */

    font:16px/32px "微软雅黑",Arial;
    font-style:italic;

    color:#f00;

    text-align: center;

    vertical-align: bottom;
    /*行内元素之间的垂直对齐方式*/

    line-height: 32px;
    /*行高*/

    text-indent:32px;

    text-shadow: 3px 5px 1px #888;
    /*
        x-offset
        y-offset
        blur
        color
    */

    /*对于文字过长，显示省略号效果，必须先设置容器高宽*/
    white-space:nowrap;
    /*
        文本过长，是否换行
        normal 默认换行
        nowrap 不换行
    */

    overflow: hidden;
    /*
        超出隐藏
    */
    text-overflow: ellipsis;
    /*
        文字超出隐藏
        clip 默认，裁剪
        ellipsis 省略号显示
    */

}
```
# 2. box 盒模型
content(width,height) + padding + border + margin

padding: 上 右 下 左;
如果在缩写中，确实某个值，用对称方位的值代替

border: 1px solid #f00;
该种缩写，不支持上右下左的缩写方式

border-width
border-style
border-color
这三种缩写，支持上右下左分别设置
```css
.son{
    border-width: 3px 5px 2px;
    border-style: solid dashed;
    border-color: #f00 #00f;
}
```

margin:30px;
写法类似padding

# 3. :before 和 :after伪类
## 3.1. margin-top bug

* (1) 父容器增加::before选择器，content:" ";display:block;overflow:hidden;

    由于::before并不算真正的标签，不会影响到:nth-child、:first-child之类的选择器  

* (2) 在首部增加一个空div，overflow:hidden

    出现了无意义的div

* 给父容器增加 overflow:hidden

    局限性，在需要overflow做其他用途的时候，不能使用这个方法

* 给父容器增加一个小的padding值

    不容易计算，产生了无意义代码

* 把子元素的margin-top 用父元素的padding-top实现

    每次修改padding，都要重新修改height

如果不需要兼容IE9以下浏览器，推荐方案1 ::before方法
反之，用空div

另外浮动元素（float）不会产生margin-top向上传递的问题，见下节课

# 4. 作业

1. 重做本课中的practice，必须按照"正确的属性做正确的事"原则
2. Emmet自学