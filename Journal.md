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

>HOW TO LINK YOUR SCRIPT.JS FILE WITH YOUR HTML FILE:

Put this into your HTML file:
```html
<script src="script.js"></script>
```


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
An if statement (also known as an if else statement) is a statement that identifies what statement to run based on the value of a Boolean expression. If the Boolean statement is true it will run through the if statement and if the statement is false it will run through the else statement.


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
Well by using a for loop you can run a statement (you don’t have to use just one statement you can use as many statements as you want). A for loop will run repeatedly until a specified expression evaluates to false.

C# Example:
-
```c#
var counter = 12;
var tables = 1;


for (var i = 0; i < counter; i++)
{
var a = i + 1;
Console.WriteLine($"{a} x {tables} = {a * tables}");
}
/* Output:
1 x 1 = 1
2 x 1 = 2
3 x 1 = 3
4 x 1 = 4
5 x 1 = 5
6 x 1 = 6
7 x 1 = 7
8 x 1 = 8
9 x 1 = 9
10 x 1 = 10
11 x 1 = 11
12 x 1 = 12
*/
```

JavaScript Example:
-
```JS
let count = 12;
let tables = 5;

for (let i = 0; i < count; i++) {

    let a = i + 1;
    console.log(a + "x" + tables + "=" + (a * tables));

}
/* Output:
1x5=5
2x5=10
3x5=15
4x5=20
5x5=25
6x5=30
7x5=35
8x5=40
9x5=45
10x5=50
11x5=55
12x5=60
*/
```

Do Loop
-
A do loop is a loop that will go on repeatedly until the user (you) closes the loop or the loop finds false then stops. Does check condition before entering, runs at least once.

C# Example:
```c#
bool keepgoing = true;

do
{
    Console.WriteLine("I am going to get a drink soon!");
    Console.WriteLine("Do you want to keep going?y/n");
    string response = Console.ReadLine();
    if (response == "n")
    {
        keepgoing = false;
    }
}
while (keepgoing == true);
{
    Console.Readline();
}
```

JavaScript Example:
-
```js
let counter = 5;
let index = 0;

 do {

    let a = i + 1;
    console.log("This is line number " + a);

    i++

}while(index < counter);
```