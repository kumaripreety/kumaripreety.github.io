## 6. DATA TYPES

#### 1. Value Data Type

- Directly stores variable value in memory .

- Default float value is double

  ```c#
  using System;
  
  namespace Practice_CSharp
  {
      class Program
      {
          static void Main(string[] args)
          {
              Console.WriteLine("Hello World!");
  
              // char repreents UTF-16 code unit or represents the 16-bit Unicode character.
              char c = 'p';
  
              // 16 bit signed integer
              short s = 89;
  
              // integer data type -- 32 bit size
              int i = 78;
  
              // long data type 32 bit 
              long l = 898;
  
              // ulong data type is generally 
              // used for unsigned integer values 
              ulong ul = 3624573;
  
              // by default fraction value 
              // is double in C# 
              double d = 8.358674532;
  
              // for float use 'f' as suffix 
              float f = 3.7330645f;
  
              // for decimal use m as suffix, other wise it will be considered as duble
              decimal dec = 389.5m;
  
              bool b = true;
  
  
              Console.WriteLine("char: " + c);
              Console.WriteLine("integer: " + i);
              Console.WriteLine("short: " + s);
              Console.WriteLine("long: " + l);
              Console.WriteLine("float: " + f);
              Console.WriteLine("double: " + d);
              Console.WriteLine("decimal: " + dec);
              Console.WriteLine("Unsinged long: " + ul);
  
          }
      }
  }
  
  ```

  #### 2. Reference Data Type

  - The Reference Data Types will contain a memory address of variable value because the reference types won’t store the variable value directly in memory. The built-in reference types are **string, object.**

  ##### String :

  - It represents a sequence of Unicode characters and its type name is

  ##### Object :

  * In C#, all types, predefined and user-defined, reference types and value types, inherit directly or indirectly from Object. So basically it is the base class for all the data types in C#. Before assigning values, it needs type conversion. When a variable of a value type is converted to object, it’s called **boxing**. When a variable of type object is converted to a value type, it’s called **unboxing**. Its type name is **System.Object**.

  ##### 3. Pointer Data Type :

  - The Pointer Data Types will contain a memory address of the variable value.
    - To get the pointer details we have a two symbols **ampersand (&) and asterisk (\*)**.
      

  ```
  type* identifier;
  ```

  **Example :**

  ```
  int* p1, p;   // Valid syntax
  int *p1, *p;   // Invalid 
  ```