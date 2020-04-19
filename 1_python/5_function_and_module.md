# Function And Module

##### Lamda 

- Lamda function is a function without name.

- It starts with lamda

  ```python
  L = [10, 20, 30, 40]
  y = (lambda *i: i - 2)(*L)
  x = [(lambda i: i * i)(a) for a in range(10)]
  ```

  

##### Module

> [Module]() - Contains function defination,  [package]() - Collection of modules,  [framework]() - Common implemented functionality
>
> **NOTE:** directory with init file is package. 

- [Ways to import custom module]():

  1. To import modules in our program, create a user variable `PYTHONPATH` with the path where all the modules are being stored.

  2. append `lib` folder path in `sys` and then import module

     ```python
     sys.append('C:\Users\bh815e\Documents\Personal_Docs\training\lib')
     import add_module
     ```


##### Decorator Function

- Used when we need to repition of certain portion of function in multiple function.

- It is also called as `First Class Function` (Function taking function as argument) or closures

- suppose func2 is inside func1 and x is local variable of func1, and we usle nonlocal x in func2, then even though func1 executed successfully x won't go for garbage collection. such function are called `Closures`

  

```python 
# decorator


def my_decorator(func):
    def decorated_function(x, y):
        print('Result is:')
        func(x, y)
        print('End of result')
    return decorated_function


def add1(a, b):
    print('result is:')
    print(a + b + a)
    print('end of result')


def sub1(a, b):
    print('Result is')
    print(a + b - a)
    print('end of result')

# same result as add1
@my_decorator
def add2(a, b):
    print(a + b + a)

@my_decorator
def sub2(a, b):
    print(a + b - a)

def add3(x, y):
    print(x + y)

add1(10, 20)
sub1(10, 20)

add2(10, 20)
sub2(10, 20)
f=my_decorator(add3)
# Now f will point to decorated function
f(10, 20) # Now decorated function will take 10, 20 as argument print the result

```





