DOM：文档对像模型（整个HTML文件）

# CSS框模型
>盒子模型（Box Modle）

div
1.content(内容)
2.border（边框）
3.padding（内边距）、margin（外边距）上右下左

    div {
         -webkit-box-sizing: border-box;
         -moz-box-sizing: border-box;
          box-sizing: border-box;
         }
>定位

1.相对定位
  相对于原本所在的位置，不会影响其他元素所在位置。
2.绝对定位
  与相对定位相比，不占据空间，脱离了文档流，绝对定位相对于已定位的祖先元素，如果没有祖先元素则相对于最近的包含块。
  z-index 可以调整位置

# 如何做一个网页

>1.画轮廓

定位技术+盒子技术
浮动技术：float：方向
清除浮动：clear: both;

>2.填充内容



