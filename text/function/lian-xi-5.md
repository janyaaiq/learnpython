# 练习5

```python
from numpy import *
random.seed(5)
array = random.randint(3000,size=500)
list1 = array.tolist()
array1 = random.randint(100,size=20)
list2 = array1.tolist()
```

上面这段代码生成了一个长度为500的列表list1，

1. 请写一个函数，使用for循环，将list1所有奇数提取出来，并添加到新列表list3中。
2. 请写一个函数，使用for循环遍历list2的元素，如果list2的元素同时存在于list1中，则将该元素添加到新列表list4中。



