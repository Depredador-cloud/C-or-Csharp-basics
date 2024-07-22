# C-or-Csharp-basics
# Introduction to C# Programming Language

C# (pronounced "C-sharp") is a modern, object-oriented programming language developed by Microsoft. It is part of the .NET framework and is designed for building a wide range of applications, from web applications to mobile apps to enterprise software. Here is a basic guide to the C# programming language, covering essential concepts and providing examples.

## Key Features of C#
1. **Object-Oriented**: C# supports object-oriented programming, which includes encapsulation, inheritance, and polymorphism.
2. **Type-Safe**: C# ensures type safety, which means that the code only accesses the types it is meant to, reducing errors.
3. **Component-Oriented**: C# supports component-oriented programming, making it easy to build and reuse components.
4. **Modern Language Constructs**: C# includes modern language features such as properties, events, and garbage collection.
5. **Cross-Platform**: With .NET Core, C# applications can run on multiple platforms, including Windows, macOS, and Linux.

## Basic Structure of a C# Program
A typical C# program consists of the following components:
1. **Namespace Declaration**: Namespaces are used to organize code and prevent naming conflicts.
2. **Class Declaration**: Classes are the building blocks of C# programs.
3. **Main Method**: The `Main` method is the entry point of a C# program.
4. **Statements and Expressions**: These perform operations and compute values.
5. **Variables and Data Types**: C# supports various data types, such as `int`, `float`, `double`, `char`, `string`, and more.

### Example of a Simple C# Program
```csharp
using System;

namespace HelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            // Variable declaration
            int num;

            // Print a message to the console
            Console.WriteLine("Enter a number: ");

            // Read input from the user
            num = Convert.ToInt32(Console.ReadLine());

            // Print the entered number
            Console.WriteLine("You entered: " + num);
        }
    }
}
```

### Explanation of the Example
- `using System;`: Includes the System namespace.
- `namespace HelloWorld { ... }`: Defines a namespace called `HelloWorld`.
- `class Program { ... }`: Defines a class called `Program`.
- `static void Main(string[] args) { ... }`: The `Main` method is the entry point of the program.
- `Console.WriteLine("Enter a number: ");`: Prints a message to the console.
- `num = Convert.ToInt32(Console.ReadLine());`: Reads input from the user and converts it to an integer.
- `Console.WriteLine("You entered: " + num);`: Prints the entered number to the console.

## Common Data Types in C#
- `int`: Used to store integers.
- `float`: Used to store floating-point numbers.
- `double`: Used to store double-precision floating-point numbers.
- `char`: Used to store single characters.
- `string`: Used to store sequences of characters.
- `bool`: Used to store Boolean values (`true` or `false`).

### Examples of Variables and Data Types
```csharp
using System;

namespace DataTypes
{
    class Program
    {
        static void Main(string[] args)
        {
            int age = 25;
            float height = 5.9f;
            char initial = 'M';
            string name = "John";
            bool isStudent = true;

            Console.WriteLine("Age: " + age);
            Console.WriteLine("Height: " + height);
            Console.WriteLine("Initial: " + initial);
            Console.WriteLine("Name: " + name);
            Console.WriteLine("Is Student: " + isStudent);
        }
    }
}
```

## Control Structures
C# supports various control structures for decision making and looping:
- **if, else if, else**: Used for conditional branching.
- **switch**: Used for multi-way branching.
- **for, while, do-while**: Used for looping.

### Example of Control Structures
```csharp
using System;

namespace ControlStructures
{
    class Program
    {
        static void Main(string[] args)
        {
            int num = 10;

            // if-else statement
            if (num > 0)
            {
                Console.WriteLine("Number is positive");
            }
            else
            {
                Console.WriteLine("Number is not positive");
            }

            // for loop
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine("Iteration " + i);
            }
        }
    }
}
```

### Explanation of Control Structures
- **if-else statement**: Checks if `num` is greater than 0 and prints a message accordingly.
- **for loop**: Iterates from 0 to 4, printing the iteration number each time.

## Object-Oriented Programming in C#
C# is an object-oriented language and supports the principles of object-oriented programming (OOP):
- **Encapsulation**: Bundling data and methods that operate on the data within a single unit, typically a class.
- **Inheritance**: Deriving new classes from existing ones, promoting code reuse.
- **Polymorphism**: Allowing methods to do different things based on the object it is acting upon.

### Example of a Class
```csharp
using System;

namespace OOP
{
    class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }

        public void Introduce()
        {
            Console.WriteLine("Hello, my name is " + Name + " and I am " + Age + " years old.");
        }
    }

    class Program
    {
        static void Main(string[] args)
        {
            Person person = new Person();
            person.Name = "John";
            person.Age = 30;
            person.Introduce();
        }
    }
}
```

### Explanation of the Class Example
- **Person Class**: Defines a class with two properties (`Name` and `Age`) and a method (`Introduce`).
- **Introduce Method**: Prints a greeting message using the `Name` and `Age` properties.
- **Main Method**: Creates an instance of the `Person` class, sets the properties, and calls the `Introduce` method.

## Methods in C#
Methods are blocks of code that perform specific tasks and can be reused throughout the program.

### Example of a Method
```csharp
using System;

namespace Methods
{
    class Program
    {
        static void Main(string[] args)
        {
            int result = Add(5, 3);
            Console.WriteLine("The sum is: " + result);
        }

        static int Add(int a, int b)
        {
            return a + b;
        }
    }
}
```

### Explanation of the Method Example
- **Add Method**: A static method that takes two integers as parameters and returns their sum.
- **Main Method**: Calls the `Add` method with arguments 5 and 3 and prints the result.

## Conclusion
C# is a powerful and versatile programming language that supports modern programming practices. Its object-oriented nature, strong type safety, and rich set of libraries make it a popular choice for a wide range of applications. By understanding the basic structure, data types, control structures, and object-oriented principles in C#, you can start building your own applications and explore the vast possibilities that C# programming offers.

For more detailed information and advanced topics, refer to "C# 7.0 in a Nutshell: The Definitive Reference" by Joseph Albahari and Ben Albahari, "Pro C# 7: With .NET and .NET Core" by Andrew Troelsen and Philip Japikse, and "Clean Architecture: A Craftsman's Guide to Software Structure and Design" by Robert C. Martin.

## GitHub Badge
[![C#](https://img.shields.io/badge/C%23-%23239120.svg?style=for-the-badge&logo=c-sharp&logoColor=white)](https://github.com/Depredador-cloud/Csharp-programming-basics/blob/main/README.md)


## Advanced Concepts in C#

To further enhance your understanding of C# programming, let's explore some advanced concepts that are commonly used in C# development.

### Properties
Properties in C# provide a flexible mechanism to read, write, or compute the values of private fields. They can be used as if they are public data members, but they include logic for getting and setting values.

```csharp
using System;

namespace Properties
{
    class Person
    {
        private string name;
        public string Name
        {
            get { return name; }
            set { name = value; }
        }

        public int Age { get; set; }

        public void Introduce()
        {
            Console.WriteLine($"Hello, my name is {Name} and I am {Age} years old.");
        }
    }

    class Program
    {
        static void Main(string[] args)
        {
            Person person = new Person();
            person.Name = "Alice";
            person.Age = 25;
            person.Introduce();
        }
    }
}
```

### Indexers
Indexers allow instances of a class or struct to be indexed just like arrays.

```csharp
using System;

namespace Indexers
{
    class SampleCollection<T>
    {
        private T[] arr = new T[100];
        public T this[int i]
        {
            get { return arr[i]; }
            set { arr[i] = value; }
        }
    }

    class Program
    {
        static void Main(string[] args)
        {
            var stringCollection = new SampleCollection<string>();
            stringCollection[0] = "Hello";
            stringCollection[1] = "World";

            Console.WriteLine(stringCollection[0]); // Output: Hello
            Console.WriteLine(stringCollection[1]); // Output: World
        }
    }
}
```

### Delegates and Events
Delegates are types that represent references to methods with a particular parameter list and return type. They are used to pass methods as arguments to other methods. Events are a way to provide notifications.

```csharp
using System;

namespace DelegatesEvents
{
    public delegate void Notify();

    class ProcessBusinessLogic
    {
        public event Notify ProcessCompleted;

        public void StartProcess()
        {
            Console.WriteLine("Process Started!");
            OnProcessCompleted();
        }

        protected virtual void OnProcessCompleted()
        {
            ProcessCompleted?.Invoke();
        }
    }

    class Program
    {
        static void Main(string[] args)
        {
            ProcessBusinessLogic bl = new ProcessBusinessLogic();
            bl.ProcessCompleted += Bl_ProcessCompleted;
            bl.StartProcess();
        }

        private static void Bl_ProcessCompleted()
        {
            Console.WriteLine("Process Completed!");
        }
    }
}
```

### Asynchronous Programming
Asynchronous programming in C# is supported through `async` and `await` keywords, allowing for non-blocking operations.

```csharp
using System;
using System.Threading.Tasks;

namespace AsynchronousProgramming
{
    class Program
    {
        static async Task Main(string[] args)
        {
            await DisplayCurrentTimeAsync();
        }

        static async Task DisplayCurrentTimeAsync()
        {
            await Task.Delay(2000); // Simulate a delay
            Console.WriteLine("Current Time: " + DateTime.Now);
        }
    }
}
```

### LINQ (Language Integrated Query)
LINQ is a powerful feature for querying collections in a concise and readable manner.

```csharp
using System;
using System.Linq;

namespace LINQDemo
{
    class Program
    {
        static void Main(string[] args)
        {
            int[] numbers = { 2, 3, 4, 5 };

            var squaredNumbers = numbers.Select(x => x * x);

            Console.WriteLine("Squared numbers:");
            foreach (var num in squaredNumbers)
            {
                Console.WriteLine(num);
            }
        }
    }
}
```

### Generics
Generics allow you to define classes, methods, and interfaces with a placeholder for the data type.

```csharp
using System;

namespace Generics
{
    class GenericClass<T>
    {
        private T data;

        public GenericClass(T value)
        {
            data = value;
        }

        public void Display()
        {
            Console.WriteLine($"Data: {data}");
        }
    }

    class Program
    {
        static void Main(string[] args)
        {
            GenericClass<int> intObj = new GenericClass<int>(10);
            intObj.Display();

            GenericClass<string> stringObj = new GenericClass<string>("Hello Generics");
            stringObj.Display();
        }
    }
}
```

### Exception Handling
Exception handling in C# is done using `try`, `catch`, `finally`, and `throw` keywords.

```csharp
using System;

namespace ExceptionHandling
{
    class Program
    {
        static void Main(string[] args)
        {
            try
            {
                int[] arr = new int[5];
                arr[10] = 99; // This will cause an IndexOutOfRangeException
            }
            catch (IndexOutOfRangeException ex)
            {
                Console.WriteLine("An error occurred: " + ex.Message);
            }
            finally
            {
                Console.WriteLine("This block is executed regardless of an exception.");
            }
        }
    }
}
```

## Conclusion
C# is a versatile and powerful language that supports a wide range of programming paradigms and features. By mastering the basics and exploring advanced topics such as properties, indexers, delegates, events, asynchronous programming, LINQ, generics, and exception handling, you can build robust and efficient applications. For more in-depth information, refer to "C# 7.0 in a Nutshell: The Definitive Reference" by Joseph Albahari and Ben Albahari, "Pro C# 7: With .NET and .NET Core" by Andrew Troelsen and Philip Japikse, and "Clean Architecture: A Craftsman's Guide to Software Structure and Design" by Robert C. Martin.

## GitHub Badge
[![C#](https://img.shields.io/badge/C%23-%23239120.svg?style=for-the-badge&logo=c-sharp&logoColor=white)](https://github.com/Depredador-cloud/Csharp-programming-basics/blob/main/README.md)
