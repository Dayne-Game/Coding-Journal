C# Notes

How to add files to github
1. cd desktop
2. git init (name of folder without brackets)
3. cd (name of folder created)
4. dotnet new console
5. code .
6. Use ctrl ` (backtick) to open the intergrated terminial

To run your project go:
1. dotnet restore
2. dotnet build
3. dotnet run

To commit your files to git hub:
1. Go to GitHub website and make a new repository
2. git add .
3. git commit -m "Your commit messsage"
4. git remote add origin (url without brackets)
5. git push origin master

>*PLEASE NOTE THAT YOU DON'T PUT THE URL IN EVERYTIME YOU ONLY DO IT ONCE*

To keep adding new changes to GitHub:
1. git add .
2. git commit -m "Your Commit Message"
3. git push origin master

>*Note to self < is smaller than and > is greater than

C# Variables

To make a user input variable:
```
var UserInput = Console.ReadLine();
```

To make a variable:
```
var dayne = "dayne";
```

How to do a constant string:

A constant works exactly the same as string variable but there is one difference and that is a constant value never changes.
```
const string a = "This is the value";
```

How to do a varaible scope in C#:
```
var a = 10;

if (a <= 10 )
{
    var b = 10;
    a += b;
    Console.WriteLine($"The new value of a = {a}");
}

Console.WriteLine($"The value for variable a is now {a}"); //This will return a value
Console.WriteLine($"The value for variable b is now {b}"); //This will produce an error
```
Variables genrally can be used in the block that they are declared in and deeper, but not outside of that block.