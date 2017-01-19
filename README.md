# Visual C# and Visual Basic
_Examples of introductory concepts_



# To create and run a console application

1. Start Visual Studio.
2. On the menu bar, choose _File, New, Project._
3. The _New Project_ dialog box opens.
4. Expand _Installed_, expand _Templates_, expand _Visual C#_, and then choose _Console Application_.
5. In the _Name_ box, specify a name for your project, and then choose the _OK_ button.
6. The new project appears in _Solution Explorer_.
7. If Program.cs isn't open in the _Code Editor_, open the shortcut menu for _Program.cs_ in _Solution Explorer_, and then choose _View Code_.
8. Replace the contents of Program.cs with your code.
9. Choose the F5 key to run the project. A Command Prompt window appears that contains the line with resoults of your code.


# Comments

The characters // convert the rest of the line to a comment.
``` c# // A Hello World! program in C#. 
```
You can also comment out a block of text by enclosing it between the /* and */ characters.
```c#
/* A "Hello World!" program in C#.
This program displays the string "Hello World!" on the screen. */
```

# Main Method

A C# console application must contain a Main method, in which control starts and ends. The Main method is where you create objects and execute other methods.
The Main method is a static method that resides inside a class or a struct. You can declare the Main method in one of the following ways:

It can return void.
``` c#
static void Main()
    {
        //...
    }
```
