# FILE OPERATION

##### Write Operation:



```python
# write crates a new file if doesn't exist, if it exist it truncates the file and open
F1 = open('bin\\assets\\out.txt', 'w')
X = 10
S = 'python\n'

# We can only write string inside file, so everything
# should be converted into string first
X = str(X) + '\n'
F1.write(X)
F1.write(S)

# It will transfer data from buffer to file and connection won't be lost
F1.flush()
F1.write('hello preety \n')
L = [X, S]
F1.writelines(L)
F1.flush()
F1.close()
```



##### Write Operation:

```python
F1 = open('bin\\assets\\out.txt', 'r')

# read use seek pointer, it points to begininig of the file.
r1 = F1.read()
print(r1)

# Once the read is complete seek pointer points to end, so null value will come
r2 = F1.read()
print(r2)

# point seek manually to begining.
F1.seek(0)
print("Read file after making seek as 0")

# read entire file and return as list, one line is one element of list
print(F1.readlines())
F1.close()

# read file line wise
F1 = open('bin\\assets\\out.txt', 'r')

while True:
    line = F1.readline()
    # EOF reached
    if line == '':
        break
    print(line)

# other way to read file
F1.seek(0)
r4 = F1.readlines()
r5 = []
for i in r4:
    r5.append(i.strip())
print(r5)

# other way to read, using for
F1.seek(0)
for line in F1:
    print(line.strip())
 
# other way to read file
F1.seek(0)
L = list(F1)
t = tuple(L)
print(t)
F1.close()
```

##### Append Operation:



```python
# open the file for append
F3 = open('out2.txt', 'a')
F4 = open('out3.txt', 'a')
print(20, 'java', sep='\n', file=F3, flush=True)
```



| w       | Write                                       |
| ------- | ------------------------------------------- |
| w       | Write                                       |
| w+ (wr) | Write and Read                              |
| r       | Read                                        |
| r+ (rw) | Read and Write (write data at the begining) |
| a       | Append (append data at end of file)         |
| a+ (ar) | Append and Read                             |
|         |                                             |



