# 跳出循环

在使用循环时，有时在达到某个条件后，需要提前结束本次循环或整个循环，此时可以使用continue, break语句。

continue语句跳出本次循环，break语句跳出整个循环，一般放在if判断语句中

```python
#输出1-10中的偶数
for i in range(1,11):
    if i % 2 == 1:
        continue
    print(i,"是偶数")
```

```python

#输出列表中第一个值为2的元素索引
list1 = [1,5,8,2,0,10,40,2]
for i,v in enumerate(list1):
    if  v == 2:
        print("第一个值为2的元素索引是：",i)
        break
```

