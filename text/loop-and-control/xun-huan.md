# 循环

## 为什么需要使用循环

计算机能按照指令执行逐步计算命令，但是有很多工作是简单重复性工作。

比如：计算从1到10的和。

这些有规律重复的工作，可以使用循环语句执行，通过少量的代码，实现大量数据的循环处理。 

```python
list1 = list(range(1,11)) #定义一个包含1-10的列表list1
print(list1)  #查看列表的值
sum = 0    #初始化计算和的变量sum
for a in list1:    #循环访问list1中的元素，并赋值给变量a
    sum =  sum + a   #将sum与读取到的元素相加，并把新的相加结果赋值给sum
    print(a,sum)     #查看变量a和sum的值
print(sum)         #完成循环后，打印出加和的结果
```

### FOR循环的机制

![](../../.gitbook/assets/image-5.png)
