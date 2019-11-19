# 字符串\(String/str\)

Python中用单引号 ' 、双引号 "或三引号''' 将字符括起来形成字符串。建议统一使用双引号”来定义字符串。

```python
a = 'yucebio' #单引号
b = "yucebio" #双引号
c = '''yucebio''' #三引号
print(a,b,c)
print(type(a))
print(type(b))
print(type(c))
```

如果一个数字用引号括起来，也是一个字符串。处理数据时，常会把数字和字符串弄错，导致程序错误，因此要多加注意。

```python
a = '3'
print(a)
print(type(a))
```

由数值构成的字符串与数字可以相互转换

```python
a1 = '3'
print(type(a1))
a2 = int('3') #将str转换为int
print(type(a2))
a3 = float('3') #将str转换为float
print(type(a3))
a4 = str(3) #将int转换为str
print(type(a4))
```

字符串可以用+号连接形成新的字符串：

```python
a = "yuce"
b = "bio"
c = a + b #用+号将字符串直接连接起来
print(c)

```

#### 扩展

更多字符串相关知识，[点击](https://www.runoob.com/python3/python3-data-type.html)前往学习。

