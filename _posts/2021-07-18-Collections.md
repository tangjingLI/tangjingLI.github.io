---
layout: post
title:  "Collections"
date:   2021-07-18 18:22:36 +0800
tags: python
subtitle: 'about dict and list'

---

#### List

```python
#遍历二维数组的元素的元素

myList = [[1,2],[3,4]]
for num1, num2 in myList:
    print ( num1+num2 )
```

#### Collection

通过key访问一个dict，如果key不存在，会引发'KeyError'异常，使用Collection可以为不存在的key赋予一个默认值

```python
#dict默认的key为list

#方法一
from collections import defaultdict

d = defaultdict(list)
for k, v in s:
    d[k].append(v)

#方法二
d = {}
for k, v in s:
    d.setdefault(k,[]).append(v)


#dict的默认值为int时还可以用来计数

d = defaultdict(int)
for k in s:
    d[k] += 1

#dict默认的key为set

d = defaultdict(set)
for k, v in s:
    d[k].add(v)
```
