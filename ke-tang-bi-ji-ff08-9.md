## 浮动带来的问题

1. 子元素的浮动会造成父元素的崩塌，这种现象叫脱离标准文档流或脱标
2. 文字环绕

![](/assets/QQ截图20190318192526.png)

## 通配选择器
>所有选择器

   ‘ * ’ {
        margin：10px;
    }

## 定位

1.相对定位
  相对于**原本所在的位置**，不会影响其他元素所在位置。
  position top left
  
    position: relative;
    top: 20px;
    left: 20px;

 
  ![](/assets/QQ截图20190318192918.png)
  定位后：
  ![](/assets/QQ截图20190318193136.png)
  
2.绝对定位

    position: absolute;
    top: 60px;
    left: 60px;
    
  与相对定位相比，不占据空间，**脱离了文档流**，绝对定位相对于已**相对定位或绝对定位**的祖先元素，如果没有祖先元素为相对定位或绝对定位则相对于最近的相对定位或绝对定位的包含块。
  与浮动相比，绝对定位虽然也脱离了文档流，但**不会形成文字环绕**。
  ![](/assets/QQ截图20190318193447.png)
  
3. 静止定位/固定定位
>也脱离了文档流，但固定在浏览器的窗口上
  
    position: fixed;
    top: 60px;
    left: 60px;

![](/assets/QQ截图20190318200729.png)

![](/assets/QQ截图20190318200736.png)

## 如何做一个回到页面固定位置的超链接

1. 设置一个id 或name
2. 写一个a标签，将链接地址写作对应的id

    <a href="first">
    <a href="index.html#first"> //跳转到另一个页面

    





