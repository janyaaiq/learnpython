# 可变对象与不可变对象

python中数据类型指向的对象分为可变对象和不可变对象。

* 可变对象：list，dict等
* 不可变对象有:int, string, float, tuple, bool等

对指向可变对象的变量进行操作时，该可变对象的值会改变，但内存地址不变。

```python
a = [1,2,3]
print(id(a)) 
a[1] = 10
print(a)
print(id(a)) 
```

对指向不可变对象的变量进行操作时，该变量会指向新的对象的内存地址，不改变之前对象的值。

![](../../.gitbook/assets/image%20%283%29.png)

```python
a = 10
print(id(a)) 
a += 1
print(a)
print(id(a))
```

假如变量a是一个列表，将变量a赋值给变量b，b会指向列表的内存地址，当对a或b进行操作（非赋值操作），都会修改列表的值，但是不改变列表的内存地址。

![](../../.gitbook/assets/image%20%289%29.png)

```python
a = [1,2,3]
b = a
print(id(a)) 
print(id(b)) 
a[1] = 10
print(a)
print(id(a)) 
print(b)
print(id(b)) 
```



扩展学习：[https://www.jianshu.com/p/c5582e23b26c](https://www.jianshu.com/p/c5582e23b26c)

