<!-- TOC -->

- [1. 表单2 - 组合使用](#1-表单2---组合使用)
    - [1.1. form](#11-form)
        - [1.1.1. select](#111-select)
            - [1.1.1.1. option](#1111-option)
        - [1.1.2. datalist](#112-datalist)
            - [1.1.2.1. option](#1121-option)
        - [1.1.3. fieldset](#113-fieldset)
            - [1.1.3.1. legend](#1131-legend)
- [自学内容](#自学内容)

<!-- /TOC -->
# 1. 表单2 - 组合使用
## 1.1. form
### 1.1.1. select
选择列表

通用属性

    required

特殊属性

    size        默认为1，也就是下拉列表；否则，为滚动列表

    multiple    多选

#### 1.1.1.1. option

属性

    selected    设置为默认选中项

    disabled    设置为不可选中项

规范

    无论对于下拉里列表，还是滚动列表，最好设置一个selected

### 1.1.2. datalist

datalist vs select

datalist 必须与input结合使用,input的list属性值，需要是datalist的id

```html
datalist
<input list="data" name="city1" type="text">
<datalist id="data">
    <option value="beijing">
    <option value="shanghai">
    <option value="guangzhou">
    <option value="shenzhen">
    <option value="hangzhou">
    <option value="nanjing">
</datalist>

select
<select name="city2">
    <option value="bj">北京</option>
    <option value="sh">上海</option>
    <option value="gz">广州</option>
    <option value="sz">深圳</option>
    <option value="hz">杭州</option>
    <option value="nj">南京</option>
</select>
```
#### 1.1.2.1. option

此外，datalist中，option的写法与select有差异

### 1.1.3. fieldset

分组，对表单空间进行分组

#### 1.1.3.1. legend

与fieldset搭配使用，作为分组的标题

# 自学内容

转义字符

button标签