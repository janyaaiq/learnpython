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

使用append\(\)方法在**列表末尾**增加元素

```python
list1 = [1,2,3,4]
list1.append(10)
print(list1)
```

使用pop\(\)方法，移除列表中的一个元素（默认最后一个元素），并且返回该元素的值。

```python
#pop语法：list.pop([index=-1])
list1 = [1,2,3,4]
list1.poppop(10)
```

list.pop\(\[index=-1\]\)



