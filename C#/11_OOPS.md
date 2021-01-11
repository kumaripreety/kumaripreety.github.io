## 11. Object Oriented Programming

### 1. Classes And Objects :

```C#
    public class Dog
    {
        //Instance Variable
        //Also called as state or attribute
        public string name{get; set;} //Auto implementation property
        string breed;
        int age;
        string color;

        public Dog(string name, string breed, int age, string color) {
            this.name = name;
            this.breed = breed;
            this.age = age;
            this.color = color;
        }

        //Property or bhaviour
        //method

        public string getName() {
            return this.name;
        }

    }
```

-  In C#, a user is allowed to define a class within another class. Such types of classes are known as **nested class**. This feature enables the user to logically group classes that are only used in one place, thus this increases the use of [encapsulation](https://www.geeksforgeeks.org/c-encapsulation/), and create more readable and maintainable code.
- Insatance Variable of nested class can be accessed in outer class by creating object of outer class.
- 