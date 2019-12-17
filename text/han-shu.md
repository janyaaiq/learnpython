# 函数

**为什么要使用函数**

1. 大程序代码多，使用函数将代码模块化，便于代码管理与程序理解
2. 模块化的代码便于重复使用

**什么是函数**

实现了一个或多个功能的代码集合

**如何定义函数**

```python
#自定义列表加和函数
def sum_list(list1):
    sum = 0
    for a in list1:
        sum += a
    print()
    return sum
    
l1 = [10,20,50,30]
res = sum_list(l1)
print("列表加和函数的结果是:",res)
```

如示例中代码所示：

* 函数代码块以 **def** 关键词开头，后接函数标识符名称和圆括号 **\(\)**。
* 圆括号之间可以用于定义参数，也可为空，即不需要参数。
* 函数的第一行语句可以选择性地使用文档字符串—用于存放函数说明。
* 函数内容以冒号起始，并且缩进。
* **return \[表达式\]** 语句会结束函数，并返回一个值，即使后面有代码，也会用赋值语句可以将返回值保存到其他变量。





参考资料：[https://www.runoob.com/python3/python3-function.html](https://www.runoob.com/python3/python3-function.html)

