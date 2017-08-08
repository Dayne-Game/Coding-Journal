# C# and JavaScript Notes

How to access GitHub:
---

>*How to add files to github:*
1. cd desktop
2. git init (name of folder without brackets)
3. cd (name of folder created)
4. dotnet new console (you don't do dotnet new console for JavaScript)
5. code .
6. Use ctrl ` (backtick) to open the intergrated terminial

>*To run your project (C# Only):*
1. dotnet restore
2. dotnet build
3. dotnet run

>*How to create a .gitignore file*
1. when you are in visual Code. 
2. Create a new file called .gitignore
3. Then type it in like this:
```
obj/
bin/
.vscode/
.DS_Store
```
4. Save The file.

>*How to clone your project:*
1. Open your intergrated terminal (ctrl `)
2. Type in git clone url (get the URL off your GitHub folder you want to clone)

>*To commit your files to git hub:*
1. Go to GitHub website and make a new repository
2. git add .
3. git commit -m "Your commit messsage"
4. git remote add origin (url without brackets)
5. git push origin master

>PLEASE NOTE THAT YOU DON'T PUT THE URL IN EVERYTIME YOU ONLY DO IT ONCE!!!

To keep adding new changes to GitHub:
1. git add .
2. git commit -m "Your Commit Message"
3. git push origin master

# Operators
These are used for mathmatical equations.

1. (+) - add (addition)
2. (-) - Subtract (Subtraction)
3. (<) - Smaller than
4. (>) - greater than
5. (*) - Multiply
6. (/) - Divide
---
# Variables
A variable is a name for a value, so that we can reference to a word rather than a value

C# Variable:
---
```C#
var name = "Dayne";
```
JavaScript Variable:
---
```js
var name = "Dayne"
```
---
# Constants
A constant works the same way as a variable. But a constant value can't be changed.

C# Constant:
---
```C#
const string a = "This is the value";
```
JavaScript constant:
---
```js
const a = "This is the value"
```
---
# Let (JavaScript Only)
A let is only used by JavaScript. Let is like a variable but is used inside of a block such as a if and else statement and can only be used in that block. But you can create another let with the same name and value in another block.

```js
let a = 10;
```
---
# Text Representation
Text representation is just displaying text to the user.

C# Example:
---
```C#
Console.WriteLine("Hello World");
```
JavaScript Example:
---
```js
console.log("Hello World");
```
# If and Else Statements
These are used in C# and JavaScript as well as most other coding languages. An if and else statment cheaks to see if the statement is true or false.

C# Example:
---
```C#
if ("10" == "10")
{
    <-- Execute if it is true
}
else
{
    <-- Execute if it is False
}
```
With JavaScript there are two different types. The first one is if you use == (2 equals) it will only check the value together. But if you use (3 equals) === it checks the value and the type e.g. variable, interger etc.

JavaScript Example 1 (2 equals):
---
```js
if ("20" == 20)
{
    //Execute the true block  
}
else {
    //Execute the else block
}
```
This statement is true because the values are both the same and doesn't check the type.

JavaScript Example 2 (3 equals):
---
```js
if ("20" === 20)
{
    //Execute the true block  
}
else {
    //Execute the else block
}
```
This is going to be false because it is checking the value and the type and the type isn't the same.

---

# Loops (C# and JavaScript)

For Loop:
-
