# 逻辑运算符

假设变量 a 为 10, b为 20:

| 运算符 | 逻辑表达式 | 描述 | 实例 |
| :--- | :--- | :--- | :--- |
| and | x and y | 布尔"与" - 如果 x 为 False，x and y 返回 False，否则它返回 y 的计算值。 | \(a and b\) 返回 20。 |
| or | x or y | 布尔"或" - 如果 x 是非 0，它返回 x 的值，否则它返回 y 的计算值。 | \(a or b\) 返回 10。 |
| not | not x | 布尔"非" - 如果 x 为 True，返回 False 。如果 x 为 False，它返回 True。 | not\(a and b\) 返回 False |

当If语句中需要使用多个条件时，需要用逻辑运算符组合多个条件进行判断。

例如：输出列表\[1，2，3...20\]中，大于10的偶数。

```text
list1=list(range(1,21))
for a in list1:
    if a%2==0 and a>10:
        print("大于10的偶数:",a)
```

