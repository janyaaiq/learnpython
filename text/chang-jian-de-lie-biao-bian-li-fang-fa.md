---
description: forloop
---

# 常见的列表遍历方法

**1.列表可以使用for循环读取所有元素，进行遍历:**

```python
list1 = [1,2,3,4]
for a in list1:
    print(a)
```

**2.也可以使用索引进行遍历：**

使用[range函数](rnage-han-shu-jian-jie.md)生成一个索引序列，通过循环读取索引值，遍历list1的元素。

```python
list1 = [1,2,3,4]
for i in range(0,len(list1)): #range函数生成一个0，1，2，3的序列，对应list1四个元素的索引。
    print(list1[i])
```

**3.使用**[**枚举函数\(enumerate\)**](https://www.runoob.com/python3/python3-func-enumerate.html)**遍历索引和元素：**

enumerate函数将一个可遍历的数据\(如列表、元组或字符串\)组合为一个索引序列，同时列出数据和数据下标。**可以使用list函数将枚举结果转换为list进行查看**

```python
list1 = ["a","b","c","d"]
enu = list(enumerate(list1)) #将枚举结果转换为列表
print(enu)
print(type(enu[0]))
```

使用for循环读取列表的索引和元素：

```python
list1 = ["a","b","c","d"]
for i, a in enumerate(list1):
    print("列表索引：",i,"列表元素：",a)
```

