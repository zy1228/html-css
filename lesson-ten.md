# 初始化表单
    <form action="/login" method="post">
      ...
    </form>

# 获取不同的数据

    <input type="text" name="username">
    
除text外还有以下类型：color、date、datetime、email、month、number、range、search、teltimeurl、week

文本框：

    <textarea name="comment">Add your comment here</textarea>

单选按钮：

    <input type="radio" name="day" value="Friday" checked> Friday
    <input type="radio" name="day" value="Saturday"> Saturday
    <input type="radio" name="day" value="Sunday"> Sunday

多选按钮：

    <input type="checkbox" name="day" value="Friday" checked> Friday
    <input type="checkbox" name="day" value="Saturday"> Saturday
    <input type="checkbox" name="day" value="Sunday"> Sunday

下拉列表：

    <select name="day">
      <option value="Friday" selected>Friday</option>
      <option value="Saturday">Saturday</option>
      <option value="Sunday">Sunday</option>
    </select>
    
多选框：

    <select name="day" multiple>
      <option value="Friday" selected>Friday</option>
      <option value="Saturday">Saturday</option>
      <option value="Sunday">Sunday</option>
    </select>
    
提交按钮：

    <button name="submit">
      <strong>Send Us</strong> a Message
    </button>
    
隐藏输入：
>隐藏输入提供了一种将数据传递到服务器而不将其显示给用户的方法。隐藏输入通常用于跟踪与用户无关的代码，密钥或其他信息，但在处理表单时很有用。该信息不会显示在页面上; 但是，可以通过查看页面的源代码找到它。因此，它不应用于敏感或安全的信息。

    <input type="hidden" name="tracking-code" value="abc-123">

文件输入：

    <input type="file" name="file">

# 组织表单元素

## 使用标签
>标签为表单控件提供标题或标题，明确地将它们绑在一起，并为所有用户和辅助技术创建可访问的表单。使用label元素创建的标签应包含描述其所属输入或控件的文本。

for和id标签：
>for属性的值应id与标签对应的表单控件上的属性值相同。匹配for和id属性值将两个元素绑定在一起，允许用户单击label元素以将焦点带到正确的表单控件。

    <label for="username">Username</label>
    <input type="text" name="username" id="username">
    
label元素可以包裹表单控件，例如单选按钮或复选框。这样做可省略for和id属性。

    <label>
      <input type="radio" name="day" value="Friday" checked> Friday
    </label>

字段集：
包含相关元素，默认情况下还包含边框、轮廓，可以通过css修改。

    <fieldset>
    <legend>我是一个没有感情的标题</legend>
      <label>
        Username
        <input type="text" name="username">
      </label>
      <label>
        Password
        <input type="text" name="password">
      </label>
    </fieldset>

禁用控件：

    <label>
      Username
      <input type="text" name="username" disabled>
    </label>

提示符：

    <label>
      Email Address
      <input type="email" name="email-address" placeholder="name@domain.com">
    </label>
    


    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    

    
