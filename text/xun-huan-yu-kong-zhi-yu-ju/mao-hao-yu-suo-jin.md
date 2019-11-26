---
description: '参考资料：http://www.haimengli.com/python-mh-sj/'
---

# 冒号与缩进

在学习循环时你可能注意到了一个细节：从for循环代码中的冒号:后开始、下一行内容的前面，会空几个格，但这是为什么呢？

```python
list1 = list(range(1,11))
print(list1)
sum = 0
for a in list1:
    sum =  sum + a
    print(a,sum)
print(sum)
```

这些空格的学名叫缩进，比如我们写文章首行空两个格，这就叫首行缩进。

对于Python而言，冒号和缩进是一种语法。组成循环、判断、函数等语法的代码块。Python代码中的缩进一般使用4个空格表示。

