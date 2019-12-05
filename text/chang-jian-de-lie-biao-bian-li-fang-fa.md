---
description: forloop
---

# 常见的列表遍历方法

列表可以使用for循环读取所有元素，进行遍历:

```python
list1 = [1,2,3,4]
for a in list1:
    print(a)
```

也可以使用索引进行遍历：

使用range函数生成一个索引序列，通过循环读取索引值，遍历list1的元素。

```python
list1 = [1,2,3,4]
for i in range(0,len(list1)): #range函数生成一个0，1，2，3的序列，对应list1四个元素的索引。
    print(list1[i])
```

range函数返回一个可迭代的序列，这个序列可以用索引读取元素：

```python
a =  range(0,4)
print(a)
print(type(a))
print(a[1])
```

range返回的值可以用list函数转换为列表：

```python
list1 = list(range(0,10))
print(type(list1))
print(list1)
```

