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

C# Variables

To make a user input variable:
```
var UserInput = Console.ReadLine();
```

To make a variable:
```
var dayne = "dayne";
```