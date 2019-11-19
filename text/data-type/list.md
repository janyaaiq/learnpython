# 列表（List）

**List（列表） 是 Python 中使用最频繁的数据类型。**

```python
namelist = ["邓乙晓","陈前兴","吴旭君"] #初始化一个列表
print(namelist) #查看列表的第1个值
```

上面的代码中，\["邓乙晓","陈前兴","吴旭君"\]就是一个列表，"邓乙晓"、"陈前兴"、"吴旭君"都是列表中的元素。将这个列表赋值给了namelist变量。  
从上面代码可以看出，列表用方括号 \[\] 括起元素，元素之间用逗号分隔开。

**列表中元素的数据类型可以不相同，可以是数字，字符串甚至是列表（嵌套）**

```python
multilist = ["yicebio",["大数据中心","遗传咨询"],2]
print(multilist)
```

**使用索引访问列表的元素，**

```python
list1 = [1, 2, 3, 4]
print(list1[0])
print(list1[1])
print(list1[-1])
print(list1[-3])
```

索引可以为正为负，正向索引从0开始，负向索引从-1开始：

| 列表元素 | **1** | 2 | 3 | 4 |
| :---: | :--- | :--- | :--- | :--- |
| 正索引 | 0 | 1 | 2 | 3 |
| 负索引 | -4 | -3 | -2 | -1 |

**列表可以被截取**，列表被截取后返回一个包含所需元素的新列表。

```python
list1 = [1, 2, 3, 4]
print(list1[1:3])
```

**扩展学习**

更多**列表**相关知识，[点击](https://www.runoob.com/python3/python3-list.html)前往学习。

\*\*\*\*
