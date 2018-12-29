# 列表
有序列表、无序列表、描述列表

## Unordered Lists（无序列表）
    
    <ul>
      <li>Orange</li>
      <li>Green</li>
      <li>Blue</li>
    </ul>
    
效果如下：
<ul>
  <li>Orange</li>
  <li>Green</li>
  <li>Blue</li>
</ul>

## Ordered Lists（有序列表）

    <ol>
      <li>Head north on N Halsted St</li>
      <li>Turn right on W Diversey Pkwy</li>
      <li>Turn left on N Orchard St</li>
    </ol>
    
  效果如下：
<ol>
  <li>Head north on N Halsted St</li>
  <li>Turn right on W Diversey Pkwy</li>
  <li>Turn left on N Orchard St</li>
</ol>

有序列表还具有两个独有的属性：start and reversed

### start 属性
  
    <ol start="2">
      <li>Head north on N Halsted St</li>
      <li>Turn right on W Diversey Pkwy</li>
      <li>Turn left on N Orchard St</li>
    </ol>

### reversed 属性(反转)
    
    <ol reversed>
      <li>Head north on N Halsted St</li>
      <li>Turn right on W Diversey Pkwy</li>
      <li>Turn left on N Orchard St</li>
    </ol>

### Value 属性

    <ol>
      <li>Head north on N Halsted St</li>
      <li value="9">Turn right on W Diversey Pkwy</li>
      <li>Turn left on N Orchard St</li>
    </ol>

效果如下：
![](/assets/2.png)

## Nesting Lists(嵌套列表）

    <ol>
      <li>Walk the dog</li>
      <li>Fold laundry</li>
      <li>
        Go to the grocery and buy:
        <ul>
          <li>Milk</li>
          <li>Bread</li>
          <li>Cheese</li>
        </ul>
      </li>
      <li>Mow the lawn</li>
      <li>Make dinner</li>
    </ol>

效果如下：
<ol>
  <li>Walk the dog</li>
  <li>Fold laundry</li>
  <li>Go to the grocery and buy:
    <ul>
      <li>Milk</li>
      <li>Bread</li>
      <li>Cheese</li>
    </ul>
  </li>
  <li>Mow the lawn</li>
  <li>Make dinner</li>
</ol>

# 使用CSS改变列表的样式
>list-style-type属性

源代码：

    ul {
      list-style-type: square;
    }
  
常用的值有：
<ul>
<li>none  没有列表项</li>

<li>disc  一个圆圈</li>

<li>circle  一个空心圆圈</li>

<li>square  一个满满的广场</li>

<li>decimal  十进制数</li>

<li>decimal-leading-zero  由初始零填充的十进制数字</li>

<li>lower-roman	  小写罗马数字</li>

<li>upper-roman	  大写罗马数字</li>

<li>lower-greek	  小写古典希腊语</li>

<li>lower-alpha / lower-latin	小写ASCII字母</li>

<li>upper-alpha / upper-latin	大写ASCII字母</li>

<li>armenian	传统的亚美尼亚编号</li>

<li>georgian	传统的格鲁吉亚编号  </li>

</ul>

## Horizontally Displaying List（水平）
>将display属性值更改为inline或时inline-block

    li {
      display: inline-block;
      margin: 0 10px;
    }
 
## Floating List
>设置浮动比直接删除Display的属性值更优

    li {
      float: left;
      margin: 0 20px;
    }
    



   
    


























