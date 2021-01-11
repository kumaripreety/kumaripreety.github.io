## 8. ENUM

- Mainly used to assign the names or string values to integral constants, that make a program easy to read and maintain.

- Enums are enumerated data type in C#.

- Enums are not for end-users, they are meant for developers.

- Enums are strongly typed constants. They are strongly typed, i.e., an enum of one type may not be implicitly assigned to an enum of another type even though the underlying value of their members are the same.

- Enumerations (enums) make your code more readable and understandable.

- enum values are fixed. enum can be displayed as a string and processed as an integer.

- The default type is int, and the approved types are byte, sbyte, short, ushort, uint, long, and ulong.

- Every enum type automatically derives from System.Enum and thus we can use System.Enum methods on enums.

- Enums are value types and are created on the stack and not on the heap.

- default value of enum is 1+last enum's value

  ```C#
  enum color { 
        
      // enum data members 
      Red, 
      Yellow, 
      Blue, 
        
      // assigning value yellow(1) + 5 
      Green = Yellow + 5, 
      Brown, 
        
      // assigning value Green(6) + 3 
      Black = Green + 3 
    
  } 
  ```

  