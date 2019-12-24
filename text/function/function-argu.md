# 函数的参数

#### 位置参数

power\(x,n\)函数有两个参数：x和n，这两个参数都是位置参数.

**调用函数时，传入的两个值按照位置顺序依次赋给参数x和n。**

或者直接在调用时，对参数x,n赋值，此时可以不考虑参数顺序。

```python
def power(x,n):
    '''计算x的n次乘方'''
    s = x
    for i in range(1,n):
        s = s * x
    return s

print(power(10,2))
print(power(2,3))
print(power(n3,3))
```



也可以直接对参数赋值，

#### 默认参数

对于



扩展学习：[https://www.liaoxuefeng.com/wiki/897692888725344/897693568201440](https://www.liaoxuefeng.com/wiki/897692888725344/897693568201440)

