# Training

- interpreting language
- interprates line by line
- source code + machine info  ---> Machine code
- test.py --> IC(Byte code) + M/c Info
- python virtual machine will take care of converting to byte code and running code
- suppose we import 1.py and 2.py then it will create bytecode of these imported files and store it in hard disk as well

  - pycache folder will be created to store 1.pyc and 2.pyc file
  - 2nd time onward if modified time of 1.pyc is greater than 1.py then it won't create 1.pyc again.
- Plateform independent code
- speedup execution
- can be used as procedural , functional and ooop.
- complete object oriented programming
- all objects are stored in heap
- all references and primitive data type will be stored in stack
- 

### Releases

- Directly provide source code
- executables -> pyinstaller
- zip, whil, msi, rpm etc

### Core Data Types

1. Number --- Immutable

2. String    --- Immutable

3. List

4. Tuple (can't be modified) -- Immutable 

   1. Can be used as master list of server
   2. If we want to send data from db to program

5. Dictionary

6. Set (store unique values)

   1. Immutable Set also known as Frozen set

      

> a = 10
>
> a = 100

| Object Space (heap) | Reference (Stack) |
| ------------------- | ----------------- |
| 100                 | a                 |
| 10                  |                   |

> Once reference counter becomes zero , it will clear the memory.
>
> Once unused memory becomes more than used memory -- automatic gabage collection will run.
>
> **Manual Garbage Collection** -- If we have huge data processing and we don't want to wait for automatic garbage collection then we use manual GC. 





###### Input Function:

```python
# input is always string
i = input("Enter your Name")
a = 10; b = 10
# eval executes the expression given as parameter
print(eval('a + b'))
```

