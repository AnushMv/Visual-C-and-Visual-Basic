# Visual C# and Visual Basic
_Examples of introductory concepts_



## To create and run a console application

1. Start Visual Studio.
2. On the menu bar, choose _File, New, Project._
3. The _New Project_ dialog box opens.
4. Expand _Installed_, expand _Templates_, expand _Visual C#_, and then choose _Console Application_.
5. In the _Name_ box, specify a name for your project, and then choose the _OK_ button.
6. The new project appears in _Solution Explorer_.
7. If Program.cs isn't open in the _Code Editor_, open the shortcut menu for _Program.cs_ in _Solution Explorer_, and then choose _View Code_.
8. Replace the contents of Program.cs with your code.
9. Choose the F5 key to run the project. A Command Prompt window appears that contains the line with resoults of your code.


## Comments

The characters // convert the rest of the line to a comment.
``` c# // A Hello World! program in C#. 
```
You can also comment out a block of text by enclosing it between the /* and */ characters.
```c#
/* A "Hello World!" program in C#.
This program displays the string "Hello World!" on the screen. */
```

## Main Method

A C# console application must contain a Main method, in which control starts and ends. The Main method is where you create objects and execute other methods.
The Main method is a static method that resides inside a class or a struct. You can declare the Main method in one of the following ways:

- [x] It can return void.
``` c#
static void Main()
    {
        //...
    }
```
- [x] It can return an integer.
``` c#
static int Main()
    {
        //...
        return 0;
    }
```
- [x] With either of the return types, it can take arguments.
``` c#
static void Main(string[] args)
    {
        //...
    }
```
or

``` c#
static int Main(string[] args)
    {
        //...
        return 0;
    }
```
The parameter of the Main method, args, is a string array that contains the command-line arguments used to invoke the program. The array does not include the name of the executable (exe) file.
The call to ReadKey at the end of the Main method prevents the console window from closing before you have a chance to read the output when you run your program in debug mode, by pressing F5.

## Input and Output

C# programs generally use the input/output services provided by the run-time library of the .NET Framework. The statement System.Console.WriteLine(); uses the WriteLine method. This is one of the output methods of the Console class in the run-time library. It displays its string parameter on the standard output stream followed by a new line. Other Console methods are available for different input and output operations. If you include the using System; directive at the beginning of the program, you can directly use the System classes and methods without fully qualifying them. For example, you can call Console.WriteLine instead of System.Console.WriteLine:
``` c#
using System;

Console.WriteLine();
```










