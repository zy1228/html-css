# 如何编写一个好的代码
>HTML

1.代码编写要符合标准
2.利用语义元素
3.使用正确的结构
4.遵循以下规则
  (1) 使用小写字母编写元素名称，属性和值中
  (2)缩进嵌套元素
  (3)严格使用双引号，而不是单引号或完全省略引号
  (4)移除自闭合元件末端的正斜杠
  (5)省略布尔属性的值 
5.ID和类的命名要与内容相关
6.图像应始终包含alt属性。  //这是什么东东
     <img src="puppy.jpg" alt="A beautiful, two-year-old hound mix puppy">
7.内容与样式分开写
8.保持代码精益并减少标记，尽可能将多种样式绑定到单个元素
9.在编辑页面时根据需要删除旧代码和样式

>CSS

1.使用注释顶部构建目录

    /* Primary header */
    header { ... }

2.尽量要将代码写在同一行，在符号后面加一个空格（如{、：）
3.命名尽量和内容相关
4.选选择器不要过长
5.必要时使用特定类
6.使用速记属性和值
注：但当只有一个属性时就不需要使用

    img {
          margin: 5px 10px;
        }
        
    button {
              padding-left: 20px;
           }

7.使用三字符速记十六进制颜色值，并始终在任何十六进制颜色值中使用小写字符

    .module {
              background: #ddd;
              color: #f60;
            }

8.将零值的单位删除
9.代码要对齐
10.如果样式一样，就不要重复去写




