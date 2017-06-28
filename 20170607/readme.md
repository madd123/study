<!-- TOC -->

- [1. 寻址方式 URL](#1-寻址方式-url)
- [2. iframe](#2-iframe)
- [3. ul/ol](#3-ulol)
    - [3.1. 问题](#31-问题)
- [4. DIV](#4-div)
- [5. SPAN](#5-span)
- [6. a](#6-a)
- [7. 锚点](#7-锚点)
- [8. HTML原则](#8-html原则)
- [作业](#作业)

<!-- /TOC -->

# 1. 寻址方式 URL

如果寻址方式，是按照当前位置进行计算，则叫**相对地址**

如果寻址方式，跟当前位置没关系，则叫**绝对地址**

/
./
../
./文件夹名字
./文件夹名字/文件名字.文件后缀

# 2. iframe

引入网页文件,可以引入其它，但是不建议

# 3. ul/ol

ul 无序列表（容器） 

```
type disc(默认，实心圆点)  circle（空心圆圈） square(实心方点)
```

ol 有序列表（容器）
```
type 1 a A i I
start 6  f  F vi VI
```

li 列表项

适用场景： 横着，形成一行 、 竖着，形成一列 的并列元素

dl 自定义列表(容器)
    dt 列表项
    dd 对于相邻（上）列表项的描述
## 3.1. 问题

多级列表怎么写

# 4. DIV

# 5. SPAN

# 6. a
链接
```html

<a href="./image.png"></a>
<a href="./test.zip">图片</a>
href 属性，为url地址，一般为网页，图片。其实，可以放任意文件，如果该文件浏览器可以直接打开，则打开。如果浏览器无法打开，即下载

<a href="mailto:xu@unnuo.com">邮件</a>
<a href="javascript:alert('123')">点击我</a>


```

# 7. 锚点

第一种写法
```html
    <a href="#anchor">点我</a>
    <a href="" name="anchor">点我</a>
```

第二种写法
```html
    <a href="#anchor">点我</a>
    <div id="anchor">锚点</div>
```


# 8. HTML原则

用正确的标签做正确的事

如果网页css文件完全去掉，也能实现良好的阅读体验

# 作业

利用锚点，实现tab切换效果

作业需要用到css属性 overflow:hidden 