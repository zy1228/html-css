# Getting to Know HTML


# Semantics(语义）
>描述HTML页面内容和结构，使页面便于管理和使用。下面介绍两个实际上没有任何语义价值的元素DIV和SPAN

# DIV和SPAN
>DIV是块级元素，SPAN是行级元素；块级元素与行级元素的区别在于块级元素会从新行开始，儿行级元素会接着原来的元素。

# Headings(标题）

><h1>Heading Level 1</h1>
<h2>Heading Level 2</h2>
<h3>Heading Level 3</h3>
<h4>Heading Level 4</h4>
<h5>Heading Level 5</h5>
<h6>Heading Level 6</h6>

# Building Structure（结构）

    <header>...</header>  //头
    <nav>...</nav>  //导航
    <article>...</article>  //文章
    <section>...</section>  //部分
    <aside>...</aside>  //边
    <footer>...</footer>  //页脚
    
# Deciding Between article, section, or div Elements

>仅为样式目的而分组，并且不为文档大纲提供值，请使用该div元素。
如果内容添加到文档大纲中并且可以单独重新分发或联合，则使用该article元素。
如果内容添加到文档大纲并表示内容的主题组，请使用该section元素。

# Creating Hyperlinks(超链接)

    <a href="http://baidu.com">百度</a>

# 绝对路径与相对路径

>相对路径和绝对路径
>相对路径： ./当前目录 ../上级目录

     <a href="about.html">About</a>

     <a href="http://www.google.com/">Google</a>

# Linking to an Email Address

     <a href="mailto:shay@awesome.com?subject=Reaching%20Out&body=How%20are%20you">Email Me</a>
     
# Opening Links in a New Window

    target="_blank"

# Linking to Parts of the Same Page

    <body id="top">
      ...
      <a href="#top">Back to top</a>
      ...
    </body>


    


    




