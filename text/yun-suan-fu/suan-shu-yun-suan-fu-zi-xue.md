# 算术运算符（自学）

假设变量a为10，变量b为20：

| 运算符 | 描述 | 实例 |
| :--- | :--- | :--- |


| + | 加 - 两个对象相加 | a + b 输出结果 30 |
| :--- | :--- | :--- |


<table>
  <thead>
    <tr>
      <th style="text-align:left">-</th>
      <th style="text-align:left">
        <p>&#x51CF; - &#x5F97;&#x5230;&#x8D1F;&#x6570;&#x6216;&#x662F;&#x4E00;&#x4E2A;&#x6570;&#x51CF;</p>
        <p>&#x53BB;&#x53E6;&#x4E00;&#x4E2A;&#x6570;</p>
      </th>
      <th style="text-align:left">a - b &#x8F93;&#x51FA;&#x7ED3;&#x679C; -10</th>
    </tr>
  </thead>
  <tbody></tbody>
</table>| \* | 乘 - 两个数相乘或是返回一个被重复若干次的字符串 | a \* b 输出结果 200 |
| :--- | :--- | :--- |


| / | 除 - x除以y | b / a 输出结果 2 |
| :--- | :--- | :--- |


| % | 取模 - 返回除法的余数 | b % a 输出结果 0 |
| :--- | :--- | :--- |


| \*\* | 幂 - 返回x的y次幂 | a\*\*b 为10的20次方， 输出结果 100000000000000000000 |
| :--- | :--- | :--- |


<table>
  <thead>
    <tr>
      <th style="text-align:left">//</th>
      <th style="text-align:left">&#x53D6;&#x6574;&#x9664; - &#x8FD4;&#x56DE;&#x5546;&#x7684;&#x6574;&#x6570;&#x90E8;&#x5206;</th>
      <th
      style="text-align:left">
        <p>9//2 &#x8F93;&#x51FA;&#x7ED3;&#x679C; 4 , 9.0//2.0 &#x8F93;&#x51FA;</p>
        <p>&#x7ED3;&#x679C; 4.0</p>
        </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>取余与取模计算的公式相似，都是x-y\*取整\(x/y\)。不同的地方是取余与取模用的取整方法不同。**取余对商向0取整，取模对商向下取整。**

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
print("正数向下取整：",quot1)
print("负数向下取整：",quot2)
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

