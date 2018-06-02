# C# Arrays and Lists

## What is an Array:
You can store multiple variables of the same type in an array data structure. You declare an array by specifying the type of its elements.

### How to Create an Array:
To define an array we use keyword var:

1. Arrays holde multiple values inside a single variable
2. Valuse can be sorted using Array.Sort(Array Name);
```c
var a = new string[6] {"Apple", "Cherry", "Banana", "Tomato", "Oranges", "Mandarin"};
```
### How to sort and Array in Alphabetical Order:
```c
Array.Sort(a);
```
### Print Array to the screen:
```c
Console.WriteLine(string.Join(", ", a));

// Output
// Apple, Banana, Cherry, Mandarin, Oranges, Tomato
```
### You can also display the array backwards:
```c
// just change the Array.Sort(a); to Array.Reverse(a);

Array.Reverse(a);
```
### You can also sort the array in Reverse Alphabetical Order
```c
Array.Sort(a); // sorts Array in Alphabetical order
Array.Reverse(a); // Reverses Array.
```
---
