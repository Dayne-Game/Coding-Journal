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
---
# While Loop
A while loop is a control flow statement that goes on repeatedly based on a given Boolean condition. The loop can also be known as a repeating if statement.
```C
while (count < 3)
{
    Random rnd = new Random();
    int result = rnd.Next(0,2);

    if (result == 1)//if the result is 1 it will show tails
    {
        Console.WriteLine("Tails");
        count = count + 1;
    }
    else
    {
        Console.WriteLine("Heads");
        count = count + 1;
    }

    Console.ReadLine();
}
```
---
# Do-Loop 
A do loop is a loop that will go on repeatedly until the user (you) closes the loop or the loop finds false then stops. Does check condition before entering, runs at least once.
```c
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
---
# For-each loop
The foreach statement executes a statement or a block of statements for each element in an instance of the type that implements the System.Collections.IEnumerable or System.Collections.Generic.IEnumerable<T> interface.
```c
      string[] fruits = new string[4] {"Apple", "Banana", "Coconut", "Mandarin"};

            foreach(var fruit in fruits) {

                Console.WriteLine(fruit); 
                
                // Apple
                // Banana
                // Coconut
                // Mandarin
            }
```
