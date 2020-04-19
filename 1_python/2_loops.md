# LOOPS

##### If Else Block:



```python
if a > b:
    print(" a greater than b")
elif a == b:
    print("Equal")
else:
    print(" a less than b")
```



##### For Loop:

```python
s = 'python'
for char in s:
    print(char)
```

>**NOTE:** Generator data structure creates object on demand, everything is stored in stack and not in heap. zip function is implemented using Generator. 

###### Range():

```python
r = range(start, end, jump)
# By default range function doesn't have __str__ or __repr__ implemented
print(list(r))
```

###### For else:

```python
comp = ['IBM', 'BOE1', 'SAP', 'BOE2']
for c in comp:
    if c.startswith('BOE'):
        print('found')
        break

# execute else only on successful completion of for loop
else:
    print('Not found')
```

>**NOTE:** Continue will skip logic after continue go to next iteration.

###### Generator Example(zip):

- zip behaviour can be achieved using for loop as well.

```python
host =  ['h1', 'h2', 'h3']
ips  =  ['ip1', 'ip2', 'ip3']
name =  ['preety', 'astik']

# zip function used to create pairs, list having minimum number of elements,
# that many number of pair will be generated
z = zip(host, ips, name)

# print zipped list
print(list(z))

# print null, as it zip is implemented using generator
print(list(z))

```

##### While Loop:

```python
a = 10
while a < 30:
    a += 10
    print(a)
else:
    print(a)
```

>**NOTE:** Use `pass` for empty block.