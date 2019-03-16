# CSS

## 选择器

1. 标签选择器

    标签名 {}
    
2. 类选择器

    .类名 {}
    
 类名可以选两个，用空格隔开

3. ID选择器

    '#ID {}'
    
4. 属性选择器
    
    [type="text"]
    {
      width:150px;
    }
    
5. 后代选择器
标签名1下的所有标签名2 

    标签名1 标签名2 {
        属性
    }
 
6. 子代选择器
标签名1下的子元素标签名2 ，其他的子元素中若有标签名2则不做处理

    标签名1 > 标签名2 {
        属性
    }
    
 那如果有两个strong
 
7. 组合选择器

    标签名1， 标签名2 {
        属性
    }

      
## 基础语法
    
![](/assets/css.png)

![](/assets/css2.png)

## 链接

链接的四种状态：

a:link - 普通的、未被访问的链接
a:visited - 用户已访问的链接
a:hover - 鼠标指针位于链接的上方
a:active - 链接被点击的时刻

a：是一种伪类选择器 （a可以不为标签，可以为类或id）
用这种伪类选择器可以在链接的不同状态显示不同的样式

    a:link {background-color:#B2FF99;}
    a:visited {background-color:#FFFF85;}
    a:hover {background-color:#FF704D;}
    a:active {background-color:#FF704D;}
    
## 盒子模型

转lesson four
























