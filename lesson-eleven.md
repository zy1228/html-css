# 表格

## 创建表

    <table>
    <caption>我是一个没有感情的标题</caption>
    <thead>
    <tr>
      <th scope="col">表头</th>
      <th scope="col">我爱学习</th>
      <th scope="col">学习使我</th>
      <th scope="col">超级快乐</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>1</td>
        <td>学习</td>
        <td>我</td>
        <td>快乐</td>
    </tr>
    </tbody>
    <tfoot>
      <tr>
        <td>我</td>
        <td>是</td>
        <td>一个</td>
        <td>尾巴</td>
      </tr>
    </tfoot>
    </table>

scope属性：col与列有关、row与行有关

## 表格的边框
>border-collapse属性确定表的边框模型。有三个值border-collapse属性：collapse，separate，和inherit。默认情况下，border-collapse属性值是separate，意味着所有不同的边框将彼此相邻堆叠，如上所述。collapse另一方面，该值将边框压缩为一个，选择表格单元格作为主要边框。

无间距

    table {
       border-collapse: collapse;
      }

有间距

    table {
      border-collapse: separate;
      border-spacing: 4px;
    }
    
只添加行边框
>last-child伪类选择器选择tr表中的最后一个元素并定位该td行中的元素，从表的最后一行中的单元格中删除底部。首先确保将表的border-collapse属性值设置为collapse另外，如果表正在使用结构元素，我们将要确保将表的最后一行预先限定为在tfoot元素内。

    table {
      border-collapse: collapse;
    }
    th,
    td {
      border-bottom: 1px solid #cecfd5;
      padding: 10px 15px;
    }
    tfoot tr:last-child td {
      border-bottom: 0;
    }
    
表格颜色交替
>nth-child带有even(偶数)或odd参数的伪类选择器来选择每个其他tr元素。

    tbody tr:nth-child(even) {
      background: #f0f0f2;
    }

对齐表格文字
>vertical-align属性接受不同的值的少数; 最流行的值是top，middle和bottom。这些值垂直定位文本相对于表格单元格，表格单元格元素或最接近的父元素，用于内联级元素。

















