#  JavaScript 使用   

    如需在 HTML 页面中插入 JavaScript，请使用 <script> 标签。
    <script> 和 </script> 会告诉 JavaScript 在何处开始和结束。
    <script> 和 </script> 之间的代码行包含了 JavaScript：
    
    <!DOCTYPE html>
    <html>
    <body>
    .
    .
    <script>
    document.write("<h1>This is a heading</h1>");
    document.write("<p>This is a paragraph</p>");
    </script>
    .
    .
    </body>
    </html>
    
# head 中的 JavaScript 函数

>我观察了一下，在head 和在body 中并没有什么区别。。

# 外部的 JavaScript 函数

    <!DOCTYPE html>
    <html>
    <body>
        <script src="myScript.js"></script>
    </body>
    </html>
    
# 访问元素
>document.getElementById(id)
    
    <p id="demo">我的第一个段落</p>
    
    <script>
    document.getElementById("demo").innerHTML="我的第一段 JavaScript";
    </script>
    

# 直接写到文档中
>document.write
    
    <script>
    document.write("<p>我的第一段 JavaScript</p>");
    </script>
    
**注：请使用 document.write() 仅仅向文档输出写内容。如果在文档已完成加载后执行 document.write，整个 HTML 页面将被覆盖！！**

    //以下是错误案例
    <!DOCTYPE html>
    <html>
    <body>
    
    <h1>我的第一张网页</h1>
    
    <p>我的第一个段落。</p>
    
    <button onclick="myFunction()">点击这里</button>
    
    <script>
    function myFunction()
    {
    document.write("糟糕！文档消失了。");
    }
    </script>
    
    </body>
    </html>

# 注意事项

1. 大小写敏感
2. 会忽略空格
3. 可以用反斜杠进行代码换行

    例：
    document.write("Hello \
    World!");

# 注释
类同c++

# 变量
>变量是储存信息的容器

变量必须以字母开头
变量也能以 $ 和 _ 符号开头（不过我们不推荐这么做）
变量名称对大小写敏感（y 和 Y 是不同的变量）

# 数据类型
向变量分配文本值时，应该用双引号或单引号包围这个值。
向变量赋的值是数值时，不要使用引号。如果用引号包围数值，该值会被作为文本来处理。

# 声明（创建） JavaScript 变量
>使用 var 关键词来声明变量

    var carname;
    
>变量赋值

    carname="Volvo";
    //或者在声明时就赋值
    var carname="Volvo";

# 好的编程习惯
>一条语句，多个变量
    
    var name="Gates", age=56, job="CEO";
    
声明也可横跨多行：

    var name="Gates",
    age=56,
    job="CEO";    

# 数字
>极大或极小的数字可以用指数形式表示

    var y=123e5;      // 12300000
    var z=123e-5;     // 0.00123

# 布尔
>布尔（逻辑）只能有两个值：true 或 false。

    var x=true
    var y=false
    
# 数组

    var cars=new Array();
    cars[0]="Audi";
    cars[1]="BMW";
    cars[2]="Volvo";
    
    //或者 
    var cars=new Array("Audi","BMW","Volvo")
    
# 对象
>对象由花括号分隔。在括号内部，对象的属性以名称和值对的形式 (name : value) 来定义。属性由逗号分隔：

    var person={firstname:"Bill", lastname:"Gates", id:5566};
    
上面例子中的对象 (person) 有三个属性：firstname、lastname 以及 id。
    
实例：

    name=person.lastname;
    name=person["lastname"];
    
# Undefined 和 Null
>Undefined 这个值表示变量不含有值，可以通过将变量的值设置为 null 来清空变量。

实例：

    cars=null;
    person=null;
    
# 声明变量类型
>当您声明新变量时，可以使用关键词 "new" 来声明其类型：

    var carname=new String;
    var x=      new Number;
    var y=      new Boolean;
    var cars=   new Array;
    var person= new Object;
    
JavaScript 变量均为对象。当您声明一个变量时，就创建了一个新的对象。

# 对象
>JavaScript 中的所有事物都是对象：字符串、数字、数组、日期，等等。
在 JavaScript 中，对象是拥有属性和方法的数据。

## 属性和方法
>属性是与对象相关的值,方法是能够在对象上执行的动作。

## 创建 JavaScript 对象

本例创建名为 "person" 的对象，并为其添加了四个属性：
实例:

    person=new Object();
    person.firstname="Bill";
    person.lastname="Gates";
    person.age=56;
    person.eyecolor="blue";

## 访问对象的属性

访问对象属性的语法是：

    objectName.propertyName
    
本例使用 String 对象的 length 属性来查找字符串的长度：

    var message="Hello World!";
    var x=message.length;
    
## 访问对象的方法

您可以通过下面的语法调用方法：
    
    objectName.methodName()
    
这个例子使用 String 对象的 toUpperCase() 方法来把文本转换为大写：
    
    var message="Hello world!";
    var x=message.toUpperCase();   
        
# 函数
>函数是由事件驱动的或者当它被调用时执行的可重复使用的代码块。

## 调用带参数的函数

在调用函数时，您可以向其传递值，这些值被称为参数；

    myFunction(argument1,argument2)

声明函数时，请把参数作为变量来声明：

    function myFunction(var1,var2)
    {
    这里是要执行的代码
    }

## 带有返回值的函数

    function myFunction()
    {
        var x=5;
        return x;
    }      

## 局部 JavaScript 变量

在 JavaScript 函数内部声明的变量（使用 var）是局部变量，所以只能在函数内部访问它。（该变量的作用域是局部的）。
可以在不同的函数中使用名称相同的局部变量，因为只有声明过该变量的函数才能识别出该变量。
只要函数运行完毕，本地变量就会被删除。

## 全局 JavaScript 变量

在函数外声明的变量是全局变量，网页上的所有脚本和函数都能访问它。

##JavaScript 变量的生存期
JavaScript 变量的生命期从它们被声明的时间开始。
局部变量会在函数运行以后被删除。
全局变量会在页面关闭后被删除。

### 向未声明的 JavaScript 变量来分配值
如果您把值赋给尚未声明的变量，该变量将被自动作为全局变量声明。
这条语句：

    carname="Volvo";
    
将声明一个全局变量 carname，即使它在函数内执行。   
  
# 运算符

类同c++

## 用于字符串的 + 运算符
‘+’ 运算符用于把文本值或字符串变量加起来（连接起来）。
如需把两个或多个字符串变量连接起来，请使用 + 运算符。

    txt1="What a very";
    txt2="nice day";
    txt3=txt1+txt2;

**注：如果把数字和字符串相加，结果将成为字符串 **       
    
# JavaScript 比较和逻辑运算符
> 比较和逻辑运算符用于测试 true 或 false。

类同c++
 === 全等于 x===5 为 true；x==="5" 为 false

例：
    
    if (age<18) document.write("Too young");
    
## 逻辑运算符

&& and
|| or
!  not

## 条件运算符
JavaScript 还包含了基于某些条件对变量进行赋值的条件运算符。

    variablename=(condition)?value1:value2 
    
例:

    greeting=(visitor=="PRES")?"Dear President ":"Dear ";
    
如果变量 visitor 中的值是 "PRES"，则向变量 greeting 赋值 "Dear President "，否则赋值 "Dear"。    
    
    
    
    

