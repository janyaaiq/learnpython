# 函数

#### **为什么要使用函数**

1. 大程序代码多，使用函数将代码模块化，便于代码管理与程序理解
2. 模块化的函数便于代码重复使用

#### **什么是函数**

实现了一个或多个功能的代码集合

#### **如何定义函数**

```python
#自定义列表加和函数
def sum_list(list1):
    '''This is a function for list summation''' #函数说明
    sum = 0
    for a in list1:
        sum += a
    print(sum)
    return sum #结束函数，返回sum值


l1 = [10,20,50,30] #定义列表
res = sum_list(l1) #调用函数 
print("列表加和函数的结果是:",res)


print(sum_list.__doc__) #查看函数说明方法1
help(sum_list) #查看函数说明方法2
```

如示例中代码所示：

* \[必选\]函数代码块以 **def** 关键词开头，后接函数标识符名称和圆括号 **\(\)**。
* \[可选\]圆括号之间可以用于定义参数，也可为空，即不需要参数。
* \[可选\]函数内的第一行可以使用三引号定义函数说明。
* \[必选\]函数内容以冒号起始，并且缩进。
* \[必选\]**return \[表达式\]** 语句会结束函数（如何return后面还有代码会跳过

  ），并返回一个值，可以用赋值语句将返回值保存到其他变量。

#### **练习**

```python
from numpy import *
random.seed(5)
array = random.randint(3000,size=500)
list1 = array.tolist()

#定义一个名为max_value_index的函数，提取列表中最大值的正向索引，并返回索引值
def max_value_index(list1):
    #在此添加函数代码 

max_index = max_value_index(list1)
print(max_index)
```



#### 扩展学习资料

[https://www.runoob.com/python3/python3-function.html](https://www.runoob.com/python3/python3-function.html)

