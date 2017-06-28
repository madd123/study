# background

## background-color 

    颜色英文名：red

    #ff0000
    rgb(255,0,0)
    rgba(255,0,0,0.5)

    #ff00ff

    hsl
    hsla 色相、饱和度、亮度、透明度

## backgournd-image

    backgournd-image:url()

    url("./images/background.jpg")
    url('./images/background.jpg')

    url(./images/background.jpg) 不推荐

## background-position

    两个参数，第一位，x轴的偏移量，第二位，y轴的偏移两

    100px   100px

    50%     50%     相对 **容器尺寸 - 图片尺寸** 的差值

                    当background-attachment:fixed 的时候
                    相对窗口尺寸计算

    left    top
    center  center  默认值
    right   bottom

## background-repeat

    repeat
    no-repeat
    repeat-x
    repeat-y
    round       拉伸  但是超出一定图片比例的时候repeat
    space             容器空间足够的时候进行repeat

## background-attachment    附着

    fixed       背景图片，固定，不随内容滚动
    scroll      默认，滚动，随内容滚动
    
## 缩写

background: color image repeat attachment position;

```css
background:#f00 url('./image.jpg') no-repeat;
background:#f00 url('./image.jpg') no-repeat center top;
```