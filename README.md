介绍：flex布局为弹性布局，灵活性很强，分主轴和交叉轴。

1、块级元素display=flex，行内元素display:inline-flex;
2、容器flex-direction控制主轴方向，主轴方向为direction方向；
    - row（默认值）：主轴为水平方向，起点在左端。
    - row-reverse：主轴为水平方向，起点在右端。
    - column：主轴为垂直方向，起点在上沿。
    - column-reverse：主轴为垂直方向，起点在下沿。
3、容器justify-content属性定义主轴方向的对齐方式；
4、容器align-items属性定义交叉轴方向的对齐方式；
5、子容器flex-grow属性定义元素的放大比例，默认为0，如果子元素该值都相同，则等比占用空间。

水平居中示例：
``` css
.box {
    display: flex;
    display: -webkit-flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
    height: 200px;
}
```
 
垂直居中示例：
``` css
.box {
    width: 100%;
    display: inline-flex;
    display: -webkit-inline-flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    height: 200px;
}
```

对比：网格布局、百分比布局、圣杯布局、流式布局
