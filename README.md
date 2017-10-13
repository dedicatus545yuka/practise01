# practise01
全局佈局  
### 昨天就要发的今天只是补上，图片这东西怎么在这修改大小啊，真是麻烦:dizzy_face:
![案例要求](http://a1.qpic.cn/psb?/V118JuTr3rHMrA/U.BSgaMOOnZ6xQuK6RyMVcWUm72g4ndVVMlvg0YWEzI!/b/dPMAAAAAAAAA&bo=GwWAAgAAAAADB74!&rf=viewer_4 =600x400)  
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>全局布局</title>
    <link rel="stylesheet" href="全局.css">
</head>
<body>
    <div class="center"></div>
    <div class="left">
        <div class="wrap"></div>
    </div>
    <div class="top"></div>
    <div class="bottom"></div>
</body>
</html>
```
`全局.css`
```css
body {
    margin: 0;
}
.top {
    width: 100%;
    height: 100px;
    background: lightcoral;
    /* 为元素设置基本样式 */
    position: fixed;
    top: 0;
    /* 开启固定定位让元素固定在指定位置 */
}
.bottom {
    width: 100% ;
    height: 100px;
    background: lightskyblue;
    position: fixed;
    bottom: 0;
    /* 开启定位让元素固定在浏览器底部  */
}
.left {
    width: 150px;
    height: 100%;
    background-color: lawngreen;
    position: fixed;
    left: 0;
    /* 开启定位让元素定位在浏览器左部 */
}
.center {
    margin: 100px 0 100px 150px;
    /* 通过设置外边距来改变元素的偏移量 */
    background-color: azure;
    border: 10px solid lightslategrey;
    float: left;
    /* 开启浮动后盒子的大小由内容来决定且不会影响到原来的页面布局*/
}
.wrap {
    width: 150px;
    position: absolute;
    top: 100px;
    bottom: 100px;
    overflow: auto;
}
```
