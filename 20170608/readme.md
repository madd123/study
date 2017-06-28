<!-- TOC -->

- [1. 表格](#1-表格)
    - [1.1. 基本标签](#11-基本标签)
    - [1.2. 基本属性](#12-基本属性)
        - [1.2.1. 练习](#121-练习)
    - [1.3. table 嵌套](#13-table-嵌套)
        - [1.3.1. 练习](#131-练习)
- [2. Div 和 Span](#2-div-和-span)
- [3. H5语义化标签](#3-h5语义化标签)
    - [3.1. 预习 表单](#31-预习-表单)

<!-- /TOC -->
# 1. 表格

## 1.1. 基本标签

table 表格
 
tr 表格行

th 表头单元格

td 普通单元格

单元格，必须在行里面，行必须写在table里面

caption 标题标签 caption不占据table的高度

thead 表头分组
tbody 表主体分组 table的高度，减去thead和tfoot的高度，剩下的有tbody根据行数平分
tfoot 表脚注分组

## 1.2. 基本属性

table:

    width,height,border,cellpadding,cellspacing
    bgcolor

tr:

    align(left center right) valign(top middle bottom)

td:

    width height align valign
    colspan 向右合并单元格
    rowspan 向下合并单元格

### 1.2.1. 练习

利用表格，和img，排版座机电话面板

## 1.3. table 嵌套

### 1.3.1. 练习

重做1.2.1的练习，每一格的数字使用表格的排版完成，模拟电子数字效果

# 2. Div 和 Span

div Division

    块级元素 block
    display:block

    默认自成一块区域，独占一行，可设置高宽

span 用来组合行内元素的

    行内元素 inline
    display:inline

    默认，相当于文字，从左到右，组成一行，不可设置高宽

img 行内块元素

    行内块元素  inline-block
    display: inline-block / inline
    与行内元素显示规则一致，但是可以设置高宽

一般，用来排版的元素，都是块级元素
一般，用来修饰文字的元素，都是行内元素

块级元素和行内元素可以相互转换，通过display属性

# 3. H5语义化标签

大部分语义化标签 本身跟div一样

table 布局麻烦

div 简单，但是阅读性不好

所以，才出现语义化标签，但是我们不推荐使用语义化标签

为了阅读性良好，保持代码风格，良好的ID和Class命名就足够了

语义化：不等于语义化标签，具有良好的语义命名，就是良好的语义化

## 3.1. 预习 表单