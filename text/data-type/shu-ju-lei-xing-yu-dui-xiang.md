# 数据类型与对象

在python中，所有数据都是使用对象来存储的。数字，字符串，列表，元组，字典等数据，都是先在内存中构建了一个对象，然后将数据存储与对象中。

  
对象有三个特性：

1. 身份：内存地址，可以用id\(\)获取
2. 类型：决定了该对象可以保存什么类型值，可执行何种操作，需遵循什么规则，可用type\(\)获取
3. 值：对象保存的真实数据

使用赋值语句时：x＝1，python内部会生成一个值为1的内存对象，该对象是int类型，变量x指向该对象的内存地址。

整个过程由python自动触发与处理，使用者无需关心。

