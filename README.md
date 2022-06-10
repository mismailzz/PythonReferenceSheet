# PythonReferenceSheet
This repository contains the fundamental reference commands for python scripting. It will be revised and improved by the time. At the moment the new learned commands will be added into it. 

<details><summary>Strings</summary>
<p>

```python
#SUBSTRING SELECTION
>>> mystring = 'abcdefgh'
>>> mystring[:]
'abcdefgh'
>>> mystring[2:]
'cdefgh'
>>> mystring[:3]
'abc'
>>> mystring[-1]
'h'
>>> mystring[1:-2]
'bcdef'
>>> mystring[-2:]
'gh'
>>> mystring[:-2]
'abcdef'
```

```python
#STEP SIZE IN STRING
>>> mystring[::1]
'abcdefgh'
>>> mystring[::2]
'aceg'
```

```python
#FORMATING 
>>> user_info = "Person name {}. Dept name {}.".format("Ismail","NOC")
>>> user_info
'Person name ismail. Dept name NOC.'
>>> user_info = "Person name {name} Dept name {dept}".format(name="Ismail", dept="NOC")
>>> user_info
'Person name Ismail Dept name NOC'
```

</p>
</details>

<details><summary>LIST</summary>
<p>

```python
#LIST FLEXIBILITY
##LIST WITH DIFFERENT TYPE OF DATA
>>> print('x' in [1,2,3,'x',[1,2,3,4],'ismail'])
True
>>> print([1,2,3,'x',[1,2,3,4],'ismail'])
[1, 2, 3, 'x', [1, 2, 3, 4], 'ismail']
>>> mylist=[1, 2, 3, 'x', [1, 2, 3, 4], 'ismail']
>>> print(mylist[-1])
ismail
```

```python
##EXTEND LIST BY ANOTHER LIST
>>> mylist2=[4,5,6,7]
>>> mylist.extend(mylist2)
>>> print(mylist)
[1, 2, 3, 'x', [1, 2, 3, 4], 'ismail', 4, 5, 6, 7]
```

```python
##POP FROM LIST
>>> print(mylist)
[1, 2, 3, 'x', [1, 2, 3, 4], 'ismail', 4, 5, 6, 7]
>>> mylist.pop()
7
```


```python
##POP FROM LIST BY INDEX
>>> print(mylist)
[1, 2, 3, 'x', [1, 2, 3, 4], 'ismail', 4, 5, 6]
>>> mylist.pop(2)
3
>>> print(mylist)
[1, 2, 'x', [1, 2, 3, 4], 'ismail', 4, 5, 6]
>>> mylist.pop(-2)
5
>>> print(mylist)
[1, 2, 'x', [1, 2, 3, 4], 'ismail', 4, 6]
```

```python
##REVERSE LIST 
>>> print(mylist)
[1, 2, 'x', [1, 2, 3, 4], 'ismail', 4, 6]
>>> mylist.reverse()
>>> print(mylist)
[6, 4, 'ismail', [1, 2, 3, 4], 'x', 2, 1]
```

```python
##NESTED LIST
>>> print(mylist)
[6, 4, 'ismail', [1, 2, 3, 4], 'x', 2, 1]
>>> print(mylist[3][1])
2
>>> print(mylist[2][1])
s
>>> print(mylist[0][1])
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'int' object is not subscriptable
>>>
```

</p>
</details>
