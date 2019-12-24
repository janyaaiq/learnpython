# 列表操作方法

#### **初始化定义列表**

* 使用方括号\[\]定义列表
* 使用list函数定义列表

```python
list1 = []
list2 = [1,2,3,4]
list3 = list(range(1,5))
```

#### **修改列表元素**

使用索引访问元素并修改

```python
list1 = [1,2,3,4]
list1[1] = 100
print(list1)
```

#### **增加列表元素**

使用append\(\)方法在**列表末尾**增加元素，将待添加的元素写在圆括号中。

```python
list1 = [1,2,3,4]
list1.append(10)
print(list1)
```

#### **移除列表元素**

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

#### 颠倒列表元素

使用reverse\(\)方法颠倒列表，**无返回值**。

```python
list1 = [1,2,3,4,5,6,7]
list1.reverse()
print(list1)
```

#### 复制列表

使用”=“赋值

使用copy\(\)方法浅拷贝

使用copy模块的deepcopy方法深度拷贝

```python
import copy
list1 = [[1,2,3],2,3,4,5,6,7]

list2 = list1  #直接赋值
list3 = list1.copy() #浅拷贝
list4 = copy.deepcopy(list1) #深度拷贝


list1.append(8)
list1[0].append(4)

print("        list1的元素是：",list1)
print("   赋值的list2的元素是：",list2)
print(" 浅拷贝的list3的元素是：",list3)
print("深度拷贝的list4的元素是：",list4)
```



扩展学习：[https://www.runoob.com/python3/python3-list.html](https://www.runoob.com/python3/python3-list.html)

浅拷贝与深度拷贝：[https://www.runoob.com/w3cnote/python-understanding-dict-copy-shallow-or-deep.html](https://www.runoob.com/w3cnote/python-understanding-dict-copy-shallow-or-deep.html)

