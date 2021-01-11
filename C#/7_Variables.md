## 7. VARIABLES

#### Types of Variables

- Local variables
- Instance variables or Non – Static Variables
- Static Variables or Class Variables
- Constant Variables -- should be initialized while declaration, can't be modified later
- Readonly Variables -- once initialized can't be modified.

#### Implicit Type Variable

##### VAR :



- Implicitly typed variables are those variables which are declared without specifying the *[.NET type](https://www.geeksforgeeks.org/c-data-types-2/)* explicitly.

- Var type is initialized automatically at compile time based on its value.

- It is not allowed to use *var* as a parameter value or return type in the method or defining it at class level etc. because the **scope of the implicitly typed variable is local**.

- Implicitly typed variables are generally declared using **var** keyword as shown below:

  ```
  var ivariable = 10; 
  ```

- In implicitly typed variables, you are not allowed to declare multiplle **var **

  in a single statement as shown below:

  ```
   var ivalue = 20, a = 30; // invalid
  ```

- It is not allowed to use *var* as a field type in class level.

- It is allowed to use the expression in **var**

  like:

  ```
  Var b-=39
  ```

- In C#, one cannot declare implicitly typed variable without any initialization like:

  ```
   var ivalue;   // invalid
  ```

- It is not allowed to use a null value in implicitly typed variable like:

  ```
   var value = null;   // invalid
  ```

- The initializer cannot contain any object or collection, it may contain a new expression that includes an object or collection initializer like:

  ```
  // Not allowed
  var data = { 23, 24, 10};
  
  // Allowed 
  var data = new int [] {23, 34, 455, 65};
  ```

- It is not allowed to initialize implicitly typed variable with different types more than one type like:

  ```
  // It will give error because
  // the type of the value is different
  // one is of string type and another
  // one is of int type
  var value = "sd" 
  value = new int[]{1, 2, };
  ```



#### Dynamic Type Variable

- The dynamic type variable is created using dynamic keyword.

- Its type is checked during runtime

  ```c#
dynamic value = 123;
  ```
  
  
  
  
  
  ​	
  
  







