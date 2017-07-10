#css3 选择器
## 属性选择器
....
.class[src="tupianlogo.png"  ]{

}
....
css2:
[attribute]

1/[attribute="text1"]text1必须是完整的属性值，就是引号里包含的所有内容
2/[attribute~="son"]意味着title属性里包含son的所有元素
3/.mon>img[src="./tupian.jpeg"]+*{
    border: 10px solid pink;
}代表选择到tupian.jpeg的所有相邻兄弟元素
4/[attribute|=value]	[lang|=en]	选择 lang 属性值以 "en" 开头的所有元素。
5/

css3:
  常用：
1/[attribute^=value]	a[src^="https"]	选择其 src 属性值以 "https" 开头的每个 <a> 元素。------以。。。开头元素
2/attribute$=value]	a[src$=".pdf"]	选择其 src 属性以 ".pdf" 结尾的所有 <a> 元素。------------以。。。结尾元素
  用处不多：
3/[attribute*=value]	a[src*="abc"]	选择其 src 属性中包含 "abc" 子串的每个 <a> 元素。-----包含。。。的中间元素
      
element：first-of-type指定element中每一组并列第一个子元素------- 不需要父容器
element：last-of-type指定element中每一组并列最后一个
从每一组并列的元素中找到第一个元素

first-child：父容器中的第一个子元素-------需要指明父容器
last-child：父容器中的最后一个-------需要指明父容器
   俩者的区别：
   first-of-type相对于并列的元素而言（同一类元素里面去找）
   first-child相对于父容器而言

   nth-child  偶数位 2n  奇数位2n+1
   ------
   .father div:nth-child(n){

   }相对于父容器而言

###浮动元素本身，是可以被浮动元素正常撑开的；


##  box-shadow
在 CSS3 中，box-shadow 用于向方框添加阴影：
##background-size
contain ----永远有一个方向不足
只要一条边达到父容器大小，就不再放大；
cover   ------永远有方向超出      （用处更多）
最小一条边达到父容器大小，另一个方向超出；
##background-origin / background-clip
origin:指定背景图从哪开始铺
默认padding-box背景图，从padding的左上角开始
    content-box背景图，从content左上角开始
    border-box背景图，从border左上角
clip：指定背景图从哪里开始裁剪

background-clip	规定背景的绘制区域。-----从哪里开始裁剪	
background-origin	规定背景图片的定位区域。----背景图从哪开始铺	
background-size	规定背景图片的尺寸。

##background-blend-mode（要有俩张图片）混合模式
当一个div需要另一个div加入进行色彩调和时