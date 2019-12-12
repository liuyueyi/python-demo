# 函数特性之lambda

> lambda 表达式... 高级的语法糖

### 1. 匿名函数 lambda

使用lambda来修饰匿名函数，一般就是一个表达式，配合map/reduce等函数使用时，可能会非常简洁

**语法**

`lambda 参数: 执行逻辑`

如针对列表中，每个数求平方后得出新的列表

```sh
>>> list(map(lambda x: x*x, range(1, 5)))
[1, 4, 9, 16]
```

将前面的求和进行改造

```sh
>>> reduce(lambda x,y:x+y, range(1, 100))
4950
```