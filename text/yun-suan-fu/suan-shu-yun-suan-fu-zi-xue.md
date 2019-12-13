# 算术运算符（自学）

假设变量a为10，变量b为20：

<table>
  <thead>
    <tr>
      <th style="text-align:center">&#x8FD0;&#x7B97;&#x7B26;</th>
      <th style="text-align:left">&#x63CF;&#x8FF0;</th>
      <th style="text-align:left">&#x5B9E;&#x4F8B;</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:center">+</td>
      <td style="text-align:left">&#x52A0; - &#x4E24;&#x4E2A;&#x5BF9;&#x8C61;&#x76F8;&#x52A0;</td>
      <td style="text-align:left">a + b &#x8F93;&#x51FA;&#x7ED3;&#x679C; 30</td>
    </tr>
    <tr>
      <td style="text-align:center">-</td>
      <td style="text-align:left">
        <p>&#x51CF; - &#x5F97;&#x5230;&#x8D1F;&#x6570;&#x6216;&#x662F;&#x4E00;&#x4E2A;&#x6570;&#x51CF;</p>
        <p>&#x53BB;&#x53E6;&#x4E00;&#x4E2A;&#x6570;</p>
      </td>
      <td style="text-align:left">a - b &#x8F93;&#x51FA;&#x7ED3;&#x679C; -10</td>
    </tr>
    <tr>
      <td style="text-align:center">*</td>
      <td style="text-align:left">&#x4E58; - &#x4E24;&#x4E2A;&#x6570;&#x76F8;&#x4E58;&#x6216;&#x662F;&#x8FD4;&#x56DE;&#x4E00;&#x4E2A;&#x88AB;&#x91CD;&#x590D;&#x82E5;&#x5E72;&#x6B21;&#x7684;&#x5B57;&#x7B26;&#x4E32;</td>
      <td
      style="text-align:left">a * b &#x8F93;&#x51FA;&#x7ED3;&#x679C; 200</td>
    </tr>
    <tr>
      <td style="text-align:center">/</td>
      <td style="text-align:left">&#x9664; - x&#x9664;&#x4EE5;y</td>
      <td style="text-align:left">b / a &#x8F93;&#x51FA;&#x7ED3;&#x679C; 2</td>
    </tr>
    <tr>
      <td style="text-align:center">%</td>
      <td style="text-align:left">&#x53D6;&#x6A21; - &#x8FD4;&#x56DE;&#x9664;&#x6CD5;&#x7684;&#x4F59;&#x6570;</td>
      <td
      style="text-align:left">b % a &#x8F93;&#x51FA;&#x7ED3;&#x679C; 0</td>
    </tr>
    <tr>
      <td style="text-align:center">**</td>
      <td style="text-align:left">&#x5E42; - &#x8FD4;&#x56DE;x&#x7684;y&#x6B21;&#x5E42;</td>
      <td style="text-align:left">a**b &#x4E3A;10&#x7684;20&#x6B21;&#x65B9;&#xFF0C; &#x8F93;&#x51FA;&#x7ED3;&#x679C;
        100000000000000000000</td>
    </tr>
    <tr>
      <td style="text-align:center">//</td>
      <td style="text-align:left">&#x53D6;&#x6574;&#x9664; - &#x8FD4;&#x56DE;&#x5546;&#x7684;&#x6574;&#x6570;&#x90E8;&#x5206;</td>
      <td
      style="text-align:left">
        <p>9//2 &#x8F93;&#x51FA;&#x7ED3;&#x679C; 4 , 9.0//2.0 &#x8F93;&#x51FA;</p>
        <p>&#x7ED3;&#x679C; 4.0</p>
        </td>
    </tr>
  </tbody>
</table>取余与取模的区别：

取余与取模计算的公式相似，都是x-y\*取整\(x/y\)。不同的地方是取余与取模用的取整方法不同。**取余对商向0取整，取模对商向下取整。在Python中，一般通过"取模计算%"获取余数, 两者不做区分。**

* **向0取整：不论正数负数，都只取小数的整数部分。如3.6取整为3，-3.6取整未-3.**
* **向下取整：当小数为正数，则取整数部分，如3.6取整为3；当小数为负数，取整数部分并减1。如-3.6，取整为-4：-3\(整数部分\)-1**

```python
#向0取整函数int
quot1 = int(2.6) #正数向0取整
quot2 = int(-2.6) #负数向0取整
print("正数向0取整：",quot1)
print("负数向0取整：",quot2)
#向下取整函数floor
from math import floor #导入floor函数
quot3 =  floor(2.6) #正数向下取整
quot4 =  floor(-2.6) #负数向下取整
print("正数向下取整：",quot3)
print("负数向下取整：",quot4)
```

取模与取余的实现代码：

```python
from math import floor
x=7
y=-3
print("%取模计算结果",x%y)

mod1=x-y*floor(x/y) #取模
print("取模计算的商：",floor(x/y))
print("取模计算的模：",mod1)

rem1=x-y*int(x/y)   #取余
print("取余计算的商：",int(x/y))
print("取余计算的余：",rem1)
```

