## 9. STATIC KEYWORD

- Foreach loop copies the data in temporary array for evaluation.

### 1. Jump Statements

- In C#, Jump statements are used to transfer control from one point to another point in the program due to some specified code while executing the program. There are five keywords in the Jump Statements:

  **break**

  **continue**

  **goto**

  **return**

  **throw**

  - The **break statement** is used to terminate the loop or statement in which it present.
  
  - **Continue statement** is used to skip over the execution part of the loop on a certain condition. 
  
  - **goto** statement is used to transfer control to the labeled statement in the program.
  
  - **throw statement**  is used to create an object of any valid exception class with the help of *new* keyword manually.
  
    ```C#
    throw new NullReferenceException("Exception Message"); 
    static public void Main() 
        { 
            int number = 20; 
            switch (number) { 
      
            case 5: 
                Console.WriteLine("case 5"); 
                break; 
            case 10: 
                Console.WriteLine("case 10"); 
                break; 
            case 20: 
                Console.WriteLine("case 20"); 
      
                // goto statement transfer  
                // the control to case 5 
                goto case 5; 
      
            default: 
                Console.WriteLine("No match found"); 
                break; 
            } 
        } 
    ```
  
    
  
    