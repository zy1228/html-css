# Adding a Background Color
>background or background-color

background属性接受在速记形式的色彩和图像，而background-color属性是严格用于设置固体的背景色。

    div {
      background-color: #b2b2b2;
    }
    //透明背景
    div {
      background-color: #b2b2b2;
      background-color: rgba(0, 0, 0, .3);
    }  
    
# Adding a Background Image
>background or background-color
  
    div {
      background-image: url("alert.png");
    }

## Background Repeat(重复）
>默认情况下，除非另有说明，否则背景图像将无限制地垂直和水平重复

关键字的值有：repeat，repeat-x（水平），repeat-y（垂直）。no-repeat（不重复）。

    div {
      background-image: url("alert.png");
      background-repeat: no-repeat;
    }
    
## Background Position
>默认位于左上角

background-position属性需要两个值：水平偏移（第一个值）和垂直偏移（第二个值）。如果仅指定了一个值，则该值用于水平偏移，垂直偏移将默认为50%。

    div {
      background-image: url("alert.png");
      background-position: 20px 10px;
      background-repeat: no-repeat;
    }

## 速记

    div {
      background: #b2b2b2 url("alert.png") 20px 10px no-repeat;
    }

#Linear Gradient Background （线性渐变背景）

    div {
      background: #466368;
      background: -webkit-linear-gradient(#648880, #293f50);
      background:    -moz-linear-gradient(#648880, #293f50);
      background:         linear-gradient(#648880, #293f50);
    }

>更改方向

    div {
      background: #466368;
      background: linear-gradient(to right bottom, #648880, #293f50);
    }

>径向渐变背景

    div {
      background: #466368;
      background: radial-gradient(#648880, #293f50);
    }

>渐变颜色停止

    div {
      background: #648880;
      background: linear-gradient(to right, #f6f1d3, #648880, #293f50);
    }

#Using Multiple Background Images

    div {
      background:  url("foreground.png") 0 0 no-repeat, url("middle-ground.png") 0 0 no-repeat, url("background.png") 0 0 no-repeat;
    }

#CSS3 Background Size
    
    div {
      background: url("shay.jpg") 0 0 no-repeat;
      background-size: auto 75%;
      border: 2px dashed #9799a7;
      height: 240px;
      width: 200px;
    }

# CSS3背景剪辑和背景原点
>background-clip属性指定背景图像将覆盖的表面区域，background-origin属性指定background-position应该来源的位置。

关键字的值：border-box，padding-box，和content-box。

    div {
      background: url("shay.jpg") 0 0 no-repeat;
      background-clip: padding-box;
      background-origin: border-box;
    }

 ![](/assets/O7DPNX6N0O0HWKAAD_]E@XX.png)   
 
 
 
 




















