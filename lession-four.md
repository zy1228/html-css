# Box Model(盒子模型)
>在进入盒子模型的学习之前，学习如何显示元素可以更好地帮助我们理解盒子模型

## How Are Elements Displayed?
>由属性display决定

每个元素都有自己默认的display属性，但有可能会被覆盖掉，常见的有block，inline，inline-block，和none。
我们可以通过声明一个新的Display的属性值去更改元素的属性值。例如值block将使该元素成为块级元素。

    p {
        display: block;
      }

## What Is the Box Model?
>根据盒子模型的概念来说，****页面中的每一个元素都是一个矩形的盒子****，它们有width, height, padding, borders, and margins.

## Working with the Box Model

    div {
          border: 6px solid #949599;
          height: 100px;
          margin: 20px;
          padding: 20px;
          width: 400px;
        }
### Width & Height

每个元素都有自己默认的宽度和高度（如：0px），元素的默认宽度取决于它的显示值，默认宽度则取决于内容。

    div {
          width: 400px;
          height: 100px;
        }

### Margin & Padding

>根据元素的不同，浏览器会应用默认的内外边距使得内容更清晰明了。

padding（内边距）：

    div {
            padding: 20px;
        }

margin（外边距）

    div {
            margin: 20px;
        }
        
>表现形式 ：

（1）当四边的值都相同时

    div {
            margin: 20px;
        }
        
（2）（top，bottom）+（left，right）
此时top，bottom的值为10px，left，right的值为20px

    div {
          margin: 10px 20px;
        }

（3）top，right，bottom，left

    div {
          margin: 10px 20px 0 15px;
        }

（4）一次设定一个值

    div {
          margin-top: 10px;
          padding-left: 6px;
        }

### Borders
>border属性需要三个值：width，style，和color。

    div {
          border: 6px solid #949599;
        }

常见的style有：solid，double，dashed，dotted，和none

>表现形式：

    div {
          border-bottom: 6px solid #949599;
        }
        
更准确一些

    div {
          border-bottom-width: 12px;
        }
 
##  Content Box
>设置一个默认的内容框

    div {
             -webkit-box-sizing: border-box;
             -moz-box-sizing: border-box;
              box-sizing: border-box;
         }




    
























































