# 函数特性之filter

> 简而言之，filter实现过滤功能

### 1. filter

过滤，同样接收两个参数，第一个为过滤函数（返回True/False，True表示保留）；第二个为可迭代的对象

如过滤数组中的所有偶数，只保留奇数

```sh
>>> def f(s):
...   return s % 2 == 1
... 
>>> list(filter(f, range(1, 10)))
[1, 3, 5, 7, 9]
```