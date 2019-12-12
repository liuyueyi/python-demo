# 函数特性之reduce

> 简而言之，reduce实现聚合功能

### 1. reduce

map相当于是顺序的执行迭代器中的元素；而reduce则是每个元素执行完毕之后，会与下一个元素一起进行计算，最终返回的是函数最终的计算结果

一个典型的case如，获取列表中元素的和

```sh 
# 首先是导入依赖
>>> from functools import reduce
>>> def f(x, y):
...   return x + y
... 
>>> reduce(f, range(1, 100))
4950
```

> 需要额外注意的是使用reduce需要引入对应的包