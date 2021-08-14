# Python Basic

## 

## 

## Array

#### list

default

```python
>>> ls=['a','b','c', 1, 2, 3]
>>> ls
['a', 'b', 'c', 1, 2, 3]
>>>
>>> ls[0]; ls[-1]
'a'
3
>>> lsls=[[1, 2], [3, 4]]
>>> lsls
[[1, 2], [3, 4]]
>>> lsls[0]
[1, 2]
>>> lsls[-1]
[3, 4]
>>> lsls[0][1]
2
>>> lsls[0][0:]
[1, 2]
>>> lsls[0][:-1]
[1]
>>> lsls*3
[[1, 2], [3, 4], [1, 2], [3, 4], [1, 2], [3, 4]]
>>> lsls+1
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: can only concatenate list (not "int") to list
>>> lsls + lsls
[[1, 2], [3, 4], [1, 2], [3, 4]]
```

split function

```python
>>> myList = 'hello word'.split()
>>> myList
['hello', 'word']
>>> type(myList)
<class 'list'>
```

join function

```python
>>> ' '.join(myList)
'hello word'
>>> myList = myList.split()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
AttributeError: 'list' object has no attribute 'split'
>>> myList
['hello', 'word']
>>> ' n '.join(myList)
'hello n word'
```

