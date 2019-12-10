# 条件判断表达式

1**.表达式（expression）**

**表达式**是值、变量和运算符的组合。 值自身也被认为是一个表达式，变量也是，因此下面都是合法的表达式：

```python
a = 10 + 4
a
4
a < 10
```

**2.布尔（Boolean）值**

布尔值只有两个值：True和False，可以将这两个值翻译成“真”和“假”。

在Python语言底层，会将布尔值True 看做1，将布尔值False看做0，尽管从表面上看，True和1、False和0是完全不同的两个值，但实际上，它们是相同的。

我们可以在jupyter进行验证。

```python
print(True == 1)
print(False == 0)
print(True + False + 20)
```

很明显，我们可以直接将True看成1，False看成0，也可以直接将True和False当成1和0用，所以True + False + 20的计算结果是21。

**3.条件判断表达式**

在Python语言中，执行if/elif判断前，会根据**条件判断表达式**的**布尔值**，判断是否要指定代码块中的语句。**如果条件判断表达式的值不是布尔值，会先转换成布尔值再判断。**每一种类型的值都可以被解释成布尔类型的值。例如，None 0 "" \(\) \[\] {} 都会被解释成布尔值中的False。

条件判断表达式通常由以下组成：

* 数值与变量
  * a\(需被定义\)
  * 10
  * True
  * False
* 比较运算
  * a &gt; b
  * a == b
  * a &lt;= b
* 逻辑运算
  * a and b
  * a or b
  * not a
* 成员运算
  * a in list1
  * a not in list1

**4.布尔值转换**

另外，我们可以用bool函数将其他类型的值转换为布尔类型的值。

```python
bool("")
bool("Hello") 
bool([]) 
bool([1,2,3])
```

我们可以看到，在前面给出的几个会被系统认为是False的值，通过bool函数的转换，会变成真正的布尔值。不过这些值是不能直接和布尔值比较的，例如，不能直接使用“\[\] == false”，正确的做法是先用bool函数将其转换为布尔值，然后再比较 bool\(\[\]\) == false

参考资料：[https://zhuanlan.zhihu.com/p/43935794](https://zhuanlan.zhihu.com/p/43935794)

