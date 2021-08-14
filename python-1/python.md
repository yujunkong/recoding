# Python 기본 문법

## String

#### type

```python
>>> type("hello")
<class 'str'>

>>> type('hello')
<class 'str'>
```

#### line breaker

```bash
>>> print('''first
... second
... third''')
first
second
third
>>>
```

#### length, index, slice

```bash
>>> word='python'
>>> len(word)
6

>>> word[0]
'p'

>>> word[0:6]
'python'

>>> word[0:]
'python'

>>> word[:5]
'pytho'

>>> word[:-2]
'pyth'
```

## Operation

#### plus, minus, division, multiplier...

```python
>>> 1+2
3

>>> 2 ** 4 # 2의 4
16

>> 5 // 3 # 몫
1

>>> 5 % 3 # 나머지
2

>>> x = 2
>>> x += 1 # 증감 연산 i++ ++i 단일증감연산 지원안
>>> x
3
```

## Conditional

#### if

```python
>>> i = 10
>>> if i<10:
...     print('true')
... elif i==10:
...     print('same')
... else:
...     print('false')
...
same
```

#### for

```python
>>> for i in [1,2,3]:
...     print(i)
...
1
2
3
```

#### range\(start, end, increment\)

```python
>>> for i in range(1,7,2):
...     print(i)
...
1
3
5
```

#### enumerate\(array\[struct\], start\)

```python
>>> fang=['b', 'c', 'd']
>>> for idx, symbol in enumerate(fang, 1):
...     print(idx, symbol)
...
1 b
2 c
3 d
```

#### while

```python
>>> i = 1
>>> while i < 7:
...     print(i)
...     i += 1
...
1
2
3
4
5
6
```

#### while else, for else

```python
>>> i = 0;
>>> while i>=0:
...     i+=1
...     if(i%2) == 0:
...             continue
...     if i>5:
...             break
...     print(i)
... else:
...     print("end while...")
...
1
3
5
```

#### try except

```python
>>> try:
...     1/0
... except Exception as e:
...     print("Exception occured : ", str(e))
...
Exception occured :  division by zero
```

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

