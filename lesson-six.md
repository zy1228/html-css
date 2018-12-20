# Working with Typography（排版）
>Typeface vs. Font是两个不同的概念

typeface 是我们所看见的字体的效果
font 是一个文件，包含typeface。是计算机所允许访问的字体文件。

# Adding Color to Text
>color

    html {
            color: #555;
    }

# Changing Font Properties
>font-family

从左侧开始，应用第一个字体。如果第一个字体不可用，则从左到右依次替代字体。

由两个或多个单词组成的字体需要用引号括起来。最后一个字体应该是一个关键字值，最常见的是sans-serif或serif。

    body {
            font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
    }
    
>font-size

    body {
            font-size: 14px;
    }

>font-style

关键字的值为：normal，italic，oblique，和inherit。
常用的是italic（将文本设置为斜体）和normal（将文本返回到其正常样式）。

    .special {
      font-style: italic;
    }

>font-variant(变形）

关键字的值为：normal，small-caps，和inherit。
常用的值是：normal和small-caps //看不懂

    .firm {
      font-variant: small-caps;
    }

>font-weight

关键字的值为：normal，bold，bolder，lighter，和inherit。
常用的是normal and bold，用于切换正常字体和粗体。

    .daring {
      font-weight: bold;
    }

数值可以从100-900
    
    .daring {
      font-weight: 600;
    }

注：在使用前我们需要确认字体是否包含我们所需的重量

>line-height(行首）

line-height最好设置为font-size属性值的1.5倍左右。（line-height to 150%或 1.5）

    body {
      line-height: 22px;
    }

也可用于垂直居中元素内的单行文本。
    
    .btn {
      height: 22px;
      line-height: 22px;
    }
    
>Shorthand Font Properties（速记）

顺序：font-style，font-variant，font-weight，font-size，line-height，和font-family。

    html {
      font: italic small-caps bold 14px/22px "Helvetica Neue", Helvetica, Arial, sans-serif;
    }

#Applying Text Properties(文本属性）
>文本属性可以决定如何对齐，修饰，缩进，转换和空格文本。

## Text Align（对齐）
>关键字的值：left，right，center，justify，和inherit。
    
    p {
      text-align: center;
    }

## Text Decoration
>关键字的值：none，underline，overline，line-through，和inherit。

    .note {
      text-decoration: underline;
    }

## Text Indent（缩进）

    p {
      text-indent: 20px;
    }

## Text Shadow
>前三个值是长度，最后一个值是颜色。

    p {
      text-shadow: 3px 6px 2px rgba(0, 0, 0, .3);
    }
    
##Text Transform
>关键字的值为：none，capitalize（第一个字母大写），uppercase（大写），lowercase（小写），和inherit

    p {
      text-transform: uppercase;
    }
        
## Letter Spacing（字母）
    
    p {
      letter-spacing: -.5em;
    }
    
## Word Spacing
    
    p {
      word-spacing: .25em;
    }        
            
# Using Web-Safe Fonts                
>建议使用以下字体   

Arial, Courier New, Courier, Garamond, Georgia Lucida Sans, Lucida Grande, Lucida, Palatino Linotype, Tahoma, Times New Roman, Times, Trebuchet, Verda

#Including Citations & Quotes(引用) 

    <cite>：用于引用广告素材作品，作者或资源
    <q>：用于简短的内联引用
    <blockquote>：块引用                
                                
                                
                                    
                                        
                                            
                                                
                                                    
                                                        
                                                            
                                                                
                                                                    
                                                                        
                                                                            
                                                                                
                                                                                    
                                                                                        
                                                                                            
                                                                                                
                                                                                                    
                                                                                                        
                                                                                                            
                                                                                                                    
