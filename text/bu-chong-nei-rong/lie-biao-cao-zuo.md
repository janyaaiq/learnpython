# 列表操作

**初始化定义列表**

* 使用方括号\[\]定义列表
* 使用list函数定义列表

```python
list1 = []
list2 = [1,2,3,4]
list3 = list(range(1,5))
```

**修改列表元素**

使用索引访问元素并修改

```python
list1 = [1,2,3,4]
list1[1] = 100
print(list1)
```

**增加列表元素**

使用append\(\)方法在**列表末尾**增加元素，将待添加的元素写在圆括号中。

```python
list1 = [1,2,3,4]
list1.append(10)
print(list1)
```

**移除列表元素**

1. 使用pop\(\)方法，移除列表中的一个元素，**并且返回该元素的值**。将待删除的元素索引写在圆括号中，不写则默认是-1
2. 使用del 语句删除列表指定索引的元素，**无返回值**。

```python
#pop方法
list1 = [1,2,3,4,5,6,7]
a = list1.pop() #移除列表中索引为-1的元素
print('移除的元素是:',a,"移除后的列表是:",list1)
b = list1.pop(0) #移除列表中索引为0的元素
print('移除的元素是:',b,"移除后的列表是:",list1)
c = list1.pop(1) #移除列表中索引为1的元素
print('移除的元素是:',c,"移除后的列表是:",list1)
```

```python
#del 语句
list1 = [1,2,3,4,5,6,7]
del list1[1]
print(list1)
```



扩展学习：[https://www.runoob.com/python3/python3-list.html](https://www.runoob.com/python3/python3-list.html)

