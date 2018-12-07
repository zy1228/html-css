# What Are HTML & CSS?（什么是HTML和CSS）
>HTML：ArHyperText Markup Languagee，超文本标记语言。
>CSS：Cascading Style Sheets，层叠样式表。

注：HTML & CSS应该写在两个不同的文件中

# Understanding Common HTML Terms
Element（元素）

    <a>
    
Tags（标签）

    <a>...<a>
    
Attributes(属性)

    <a href="http://shayhowe.com/">Shay Howe</a>

# Setting Up the HTML Document Structure
    <!DOCTYPE html>   //文档类型声明
    <html lang="en">
      <head>
        <meta charset="utf-8">
        <title>Hello World</title>
      </head>
      <body>
        <h1>Hello World</h1>
        <p>This is a web page.</p>
      </body>
    </html>

# Understanding Common CSS Terms
>selectors 选择器

    p { 样式属性：属性值 }
    例：
    p {
        color: blue;
        font-size: 6px;
      }
      
>class selectors
类选择器比类型选择器更具体，因为它们选择特定的元素组而不是一种类型的所有元素。

CSS

    .classname{
      样式属性：属性值
      }
     例：
    .baidu {
      color: blue;
      font-size: 6px;
      }
HTML

    <p class="baidu">...</p>

>ID selectors
ID选择器甚至比类选择器更精确，因为它们一次只针对一个唯一元素,id选择器和类选择器可以叠加使用

 CSS

    #id{
      样式属性：属性值
      }
     例：
    .Google {
      color: blue;
      font-size: 6px;
      }
HTML

    <p id="Google">...</p>
    
# USing Css Resets
>由于不同的浏览器样式有一定的区别，通过一个全局的样式定义，让后续的代码编写在一个统一的环境变量运行

    /* http://meyerweb.com/eric/tools/css/reset/ 2. v2.0 | 20110126
    License: none (public domain)
    */

    html, body, div, span, applet, object, iframe,
    h1, h2, h3, h4, h5, h6, p, blockquote, pre,
    a, abbr, acronym, address, big, cite, code,
    del, dfn, em, img, ins, kbd, q, s, samp,
    small, strike, strong, sub, sup, tt, var,
    b, u, i, center,
    dl, dt, dd, ol, ul, li,
    fieldset, form, label, legend,
    table, caption, tbody, tfoot, thead, tr, th, td,
    article, aside, canvas, details, embed,
    figure, figcaption, footer, header, hgroup,
    menu, nav, output, ruby, section, summary,
    time, mark, audio, video {
      margin: 0;
      padding: 0;
      border: 0;
      font-size: 100%;
      font: inherit;
      vertical-align: baseline;
    }
    /* HTML5 display-role reset for older browsers */
    article, aside, details, figcaption, figure,
    footer, header, hgroup, menu, nav, section {
      display: block;
    }
    body {
      line-height: 1;
    }
    ol, ul {
      list-style: none;
    }
    blockquote, q {
      quotes: none;
    }
    blockquote:before, blockquote:after,
    q:before, q:after {
      content: '';
      content: none;
    }
    table {
      border-collapse: collapse;
      border-spacing: 0;
    }









    



