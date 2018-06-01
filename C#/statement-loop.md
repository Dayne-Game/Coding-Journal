# C# Statement and Loops

## If Statement
```c
if ("20" == 20)
{
    // Execute the true block
} 
else
{
    // Execute the false block
}
```
### This statement is true because the values are both the same and doesn't check the type.
---
## For Loop
### Well by using a for loop you can run a statement (you don’t have to use just one statement you can use as many statements as you want). A for loop will run repeatedly until a specified expression evaluates to false.
```c 
var count = 10;

for(var i = 0; i < count; i++)
{
    Console.WriteLine("Hello World");
}
```
