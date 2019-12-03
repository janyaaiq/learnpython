# 条件控制语句

**1.常见条件控制语句：**

* if语句 单独 if 判断，条件为 True 值执行语句块，否则跳过。
* if..else..语句 当 if 的条件为 True 时执行 if 下的语句块，否则执行 else 下语句块。
* if..elif..else..语句 ****从 if 的第一个条件开始依次判断，找到条件为 True 的执行它下面的语句块，如果找不到则执行 else 语句块。

**2. if..elif..else..语句示例：**

根据年龄age判断，是中年人，成年人还是未成年人

```python
age = 30
if age >= 40:
    print(age, '岁是中年人')
    print('执行if的语句块1')
elif age >= 18:
    print(age, '岁是成年人')
    print('执行elif的语句块2')
elif age >= 3:
    print(age, '岁是儿童')
    print('执行elif的语句块3')
else:
    print(age, '岁是婴儿')
    print('执行else的语句块')
```

**当if的条件为真，执行if的语句块1，如果elif的条件也为真，不会执行【 elif 的语句块2】语句。**

**3.条件语句嵌套：**

对于前面if..elif..elif..else的条件语句，可以看成是if..else..语句嵌套的简写：

```python
age = 30
if age >= 40:
    print(age, '岁是中年人')
    print('执行if的语句块1')
else:
    if age >= 18:
        print(age, '岁是成年人')
        print('执行elif的语句块2')
    else:
        if age >= 3:
            print(age, '岁是儿童')
            print('执行elif的语句块3')
        else:
            print(age, '岁是婴儿')
            print('执行else的语句块')
```

**参考资料与扩展阅读：点击**[**链接**](https://zhuanlan.zhihu.com/p/61955676)**前往知乎查看。**

