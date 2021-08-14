# Conditional

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

