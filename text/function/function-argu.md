# 函数的参数

### 位置参数

power\(x,n\)函数有两个参数：x和n，这两个参数都是位置参数.

调用函数时，传入的两个值按照位置顺序依次赋给参数x和n。

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
print(power(n=3,x=2))
```

### 默认参数

对于有的函数，有些参数的值经常变化，有些参数的值不经常变化。这个时候可以将不经常变化的参数设置为默认参数。减少调用的时候的参数传入数量。

如power函数，由于我们经常计算 $$x^2$$ ，可以把第二个参数n的默认值设定为2：

```python
def power(x,n=2):
    '''计算x的n次乘方'''
    s = x
    for i in range(1,n):
        s = s * x
    return s

print(power(10))
print(power(2,3))
print(power(n=3,x=2))
```

默认参数需放在位置参数后面，如果放在位置参数前面，定义参数的代码会报错：

```python
def power(n=2,x):
    '''计算x的n次乘方'''
    s = x
    for i in range(1,n):
        s = s * x
    return s
```

默认参数不可使用可变对象做为默认值:

```python
def add_end(a=):
    L.append('END')
    return L
```

扩展学习：[https://www.liaoxuefeng.com/wiki/897692888725344/897693568201440](https://www.liaoxuefeng.com/wiki/897692888725344/897693568201440)

