# 数字\(Number）

最常用的Number类型有两类：

* **int\(整数类型\)**
* **float\(浮点数、小数\)**

以下是对数字数据进行变量赋值、输出、查看数据类型的操作，请在Jupyter中进行练习。

```python
a = 1 #将int数值赋值给变量a
print(a) #输出变量a的值
type(a) #查看变量a存储的数据类型

b = 1.0 #将float数字赋值给变量b
print(b) #输出变量b的值
type(b) #查看变量b存储的数据类型
```

**int和float类型可以相互转换。**

```python
a = 2.3
a = float(a) #将a的值从int型转换为float型
print(a) #输出a的值
a = int(a) #将a的值从float型转换为int型
print(a) #输出a的值
```

### 数值运算

数值运算是程序中最常用的功能。  
常见的运算规则在我们我们小学初中时都学习过，复杂的运算暂用不上，有需要的时候可以自学。请在jupyter中练习以下数值运算代码：

```python
a1 = 5 + 4  # 加法
a2 = 4.3 - 2 # 减法
a3 = 3 * 7  # 乘法
a4 = 2 / 4  # 除法，得到一个浮点数
a5 = 2 // 4 # 除法，得到一个整数
a6 = 17 % 3 # 取余 
a7 = 2 ** 5 # 乘方
print(a1,a2,a3,a4,a5,a6,a7)
```

#### 扩展

更多数字相关知识，[点击](https://www.runoob.com/python3/python3-data-type.html)前往学习。

