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

Arithmetic Operations:
-
Simple Maths within programming.

Example Variables: var a = 3; var b = 6;

1. (+) - add (addition) Example: a + b = 9
2. (-) - Subtract (Subtraction) Example: b - a = 3
3. (*) - Multiply Example: a * b = 18
4. (/) - Divide Example: b / a = 2
5. (%) - Modulus Example: a + b = 9
6. (++) - Increment by one Example: a++ (this will become 4)
7. (--) - Decrement by one Example: b- (this will become 5)

Relational Operations:
-
Relational Operators are used when we compare 2 values. These are used when using if statement and loops comparisons always give us a true false value.

8. (==) - Check if 2 values are equal Example: a + b = 9
9. (!=) - Check if 2 values are not equal Example: b - a = 3
10. (<) - Smaller than Example: a < b = true
11. (>) - greater than Example: b > a = True
12. (>=) Check if the left side is greater or equal to the right side. Example: a + b = 9
13. (<=) Check if the left side is smaller or equal to the right side Example: a++ (this will be 4).

Logical Operators:
-
Logical Operators compares 2 or more boolean values
Each Relational Operator gives a boolean value
These are also used with if statements

For the examples below assume that a = true and b = false

14. (&&) And operator-both sides have to be true. Example: (a && b) this will be false
15. (||) Or operator - Only one side needs to be true. Example: (a || b) This would be true
16. (!) Or operator - Only one side needs to be true. Example: !(a && b) this would be true.

Assignment Operators:
-
Assignment Operators sets a value to a variable
a single = is an assignment (not equals like in maths)

Assume that a = 3 and b = 6 and c = 5 as values. d will hold an answer

17. (=) Assignment Example: d = a + b (answer (d) is 9)
18. (+=) AND AND adds a value to the left operand in the equation on the right. Example: c += a; c = c + a (c = 8)
19. (-=) SUBTRACTS and removes a value from the left operand in the equation on the right Example: c -= a; c = c - a (c = 2)
20. (*=) MULTIPLIES and gets the product of the value on the left and a number on the right. Example: c *= b; c = c * b (c = 2)
21. (/=) DIVIDES and gets the division of the value on the left and a number on the right. Example: b /= 3; b = b /3 (b = 2)
22. (%=) MODULUS and gets the modulus of the value on the left and a number on the right. Example: c %= a; c = c % a (c = 2)
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
# User Input

C# Example:
-
```c#
var userInput = Console.ReadLine();
```
JavaScript Example:
-
```JS
var person = prompt("Please enter your name", "Harry Potter");
```

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
---
# Boolean 
A boolean holds a value of true or false. A boolean in javascript can be a var or let.

C# Example (using a do loop example):
-
```C#
bool keepgoing = true;

do
{
    Console.WriteLine("I am going to get a drink soon!");
    Console.WriteLine("Do you want to keep going? y/n");
    string response = Console.ReadLine();

    if (response == "n")
        keepgoing = false;
}
while (keepgoing == true);

Console.ReadLine();
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

             Console.WriteLine("Please enter a number:");
var tables = Console.ReadLine();

var isnumber = int.TryParse(tables, out int number1);



for (var i = 0; i < counter; i++)
{
var a = i + 1;
Console.WriteLine($"{a} x {number1} = {a * number1}");
}

```

JavaScript Example:
-
```JS
let count = 12;
let timestables = prompt("Please enter a number", "")



for (let i = 0; i < count; i++) {

    var tables = parseInt(timestables);

    let a = i + 1;
    console.log(a + "x" + tables + "=" + (a * tables));

}
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
var drink = function() { // Write your do/while loop here! 
    var choice = "y";
    do {

        choice = prompt("I am going to get a drink soon! Do you want me to keep going? y/n");

    } while (choice != "n");
};
drink()
```

While Loop
-
A while loop is a control flow statement that goes on repeatedly based on a given Boolean condition. The loop can also be known as a repeating if statement.

C# Example:
-
```C#
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

JavaScript Example:
-
```js
let counter = 5;
let index = 0;

while(index < counter) {

    let a = index + 1;
    console.log("This is line number " + a);

    index++
}
```
---
# NaN as a result of a loop:
NaN stands for not a number:

```js
var multiples = [1064, 256, 374, 102, "sheep", "camel"];
var newArray = [];
for (var i = 0; i < multiples.length; i++) {
//checking if it is a number
 if (!isNaN(multiples[i])) 
  {  
     console.log(multiples[i])  //showing us the number
     newArray[i] = multiples[i] //add numbers to a new array
  }
}
console.log("Only Numbers - ", newArray)
```
---
#  JavaScript Array 
Arrays work also very similar in Javascript, but there are no lists.

Create a new array:
-
```js
var multiples = [1064, 256, 374, 102, "sheep", "camel"];
```
The VIP Reference:
-
```js
var multiples = [1064, 256, 374, 102, "sheep", "camel"]; [v] (value)
index =            0    1    2    3      4        5      [i] (index)
position =       1st   2nd  3rd  4th    5th      6th     [p] (position)
```
Some extra JavaScript Methods:
-
```js
var multiples = [1064, 256, 374, 102, "sheep", "camel"];
var firstItem = multiples[0];     //1064
var length = multiples.length     //6
var allItems = multiples.join()   //"1064,256,374,102,sheep,camel"
var sorting = multiples.sort()    //102, 1064, 256, 374, "camel", "sheep"
var reverse = multiples.reverse() //"camel", "sheep", 102, 374, 256, 1064
```
Adding Items into an Array:
-
Adding to the end of the Array:
-
```js
var newLength = multiples.push('horse');
// [1064, 256, 374, 102, "sheep", "camel", "horse"]
```
Removing the last item of the array:
-
```js
var last = multiples.pop(); // remove "camel" (from the end)
```
Finding a position of an item in an array:
-
```js
var pos = multiples.indexOf('camel'); //5
```
---
# C# Arrays and Lists
```c
public static void Main(string[] args)
{
    //Create an Array
    var a = new string[6] {"Apples", "Cherry", "Bannana", "Tomato", "Oranges", "Mandarin"};

    //Sort the Array in Alphabetical Order
    Array.Sort(a);

    //Print the Array to the screen
    Console.WriteLine(string.Join(",", a));

    //Output
    //Apples, Banana, Cherry, Mandarin, Oranges, Tomato
}
```
Arrays can also be displayed backwards:
-
```c#
public static void Main(string[] args)
{
    //Create an Array
    var a = new string[6] {"Apples", "Cherry", "Bannana", "Tomato", "Oranges", "Mandarin"};

    //Sort the Array in Alphabetical Order
    Array.Reverse(a);

    //Print the Array to the screen
    Console.WriteLine(string.Join(",", a));

    //Output
    //Mandarin, Oranges, Tomato, Banana, Cherry, Apples
}
```
Just change Array.Sort(a); to Array.Reverse(a);

Sorting in reverse (Alphabetical)
-
```c#
public static void Main(string[] args)
{
    //Create an Array
    var a = new string[6] {"Apples", "Cherry", "Bannana", "Tomato", "Oranges", "Mandarin"};

    //Sort the Array in Alphabetical Order
    Array.Sort(a);
    Array.Reverse(a);

    //Print the Array to the screen
    Console.WriteLine(string.Join(",", a));

    //Output
    //Tomato, Oranges, Mandarin, Cherry, Banana, Apples
}
```
Array values can be printed in a loop or using string methods
-
```C#
public static void Main(string[] args)
{
    //Create an Array
    var a = new string[6] {"Apples", "Cherry", "Bannana", "Tomato", "Oranges", "Mandarin"};
    
    //Print the Array as a string
    var output = string.Join(",", a);

    //Print the Array to the screen
    Console.WriteLine(output);

    //Output
    //"Apples, Cherry, Banana, Tomato, Oranges, Mandarin"
}
```
Array Values can be printed in a loop or using string methods
```C#
public static void Main(string[] args)
{
    //Create an Array
    var a = "Apples are green and taste good";
    
    //Print the Array as a string
    var output = a.Split(' ');//Needs to be ' ' not " "

    //Print the Array to the screen
    Console.WriteLine(output[2]);

    //Output
    //"green"
}
```
To define an array we use the keyword var.

1. Arrays hold multiple values inside a single variable
2. Values can be sorted using Array.Sort(array name)

Lists
-
List<T> are a very similar to arrays in terms of functionality

>Remember when using lists. You need:
```c#
using system.collections.generic;
```
at the top of the page (usually under using system).

Reference is the same, but List<T> offer more options

Not having to set a length when defining them allows for adding and removing object later in the program.
```C#
var names = new list<string> {"bob," "Jack", "Salty"};

//Arrays use .Length to display their length
//List <T> uses the .Count to display their length
//Both return a number, just use the right one for the right type.
```
```C#
var names = new list<string> {"bob," "Jack", "Salty"};

//Objects can be added and removed

names.Add("Peter");
names.Remove("bob);
```
```C#
var firstname = "Carol";
var names = new List<string> {"bob," "Jack", "Sally"};

//Objects can be added and removed

names.Add(firstname);
names.Remove(firstname);

names.Remove(names[2]);
```
Lists are single dimension arrays.

Use a Tuple, if you want to take multiple parameters(new since .Net 4.0)
```C#
var names = new List<Tuple<string, int>>();
names.add(Tuple.Create("bob", 32));

names[0].Item1 //"bob"
names[0].Item2 //32
```
# TryParse
Sometimes we need to change the datatype so that we can do other things with our data.
For example when doing number conversion, we cannot do this using strings.

To be able convert strings to a numeric value (int, double, floats) we use the .Parse() method.
If we want to convert a string to a whole number we would use int.Parse(string) and store that value into a variable.

For a conversion to happen successfully the input from the user needs to be a number, or else you will get a value of 0 or a program crash.
```c#
Console.WriteLine("Please enter in a number");
var input1 = Console.ReadLine();
var number1 = int.Parse(input1);

Console.WriteLine(number1 * 2);
```
Using TryParse
-
As the name implies, a tryParse() tries to parse the string. This is a boolean operation, which returns true or false For this we need to setup 2 variables, one that holds a number (int, double, floats) and one that holds the boolean value.

```c#
//Get input from user
Console.WriteLine("Please enter in a number");
var input1 = Console.ReadLine();

//Check if the input from the user is a number
var number1 = 0;
var isNumber = int.TryParse(input1, out number1);

//If the value is a number, go on with the program, or else tell the user they made an error
if(isNumber) {
    Console.WriteLine(number1 * 2);
}
else {
    Console.WriteLine("Please type in a number next time.");
}
```

# JavaScript Parsing

To interact with data using Javascript we use alert, prompt and confirm boxes. This data can then be stored into a variable.

For now we will still show information to the console, but we could display this information in a proper website as well.

To display a message without any input we use an alert box:
```js
alert("I am an alert box!");
```
To deal with a simple choice input from a user we would use a confirm box. Next we would use an if statement to control what the program does next.
```js
var txt; 

if (confirm("Press a button!") == true) {
    txt = "You pressed OK!";
} else {
    txt = "You pressed Cancel!";
}

console.log(txt);
```
Lastly to deal with user input we would use a prompt Here the user is asked a question and that value is stored in a variable.
```js
var txt; 

var person = prompt("Please enter your name", "Harry Potter");

if (person == null || person == "") {
    txt = "User cancelled the prompt.";
} else {
    txt = "Hello " + person + "! How are you today?";
}

console.log(person);
console.log(txt);
```
Displaying Information Better
-
Javascript relies heavily on the use of functions, so that not everything happens all at once as soon as a page loads.

How functions work will be explained in more detail, for now use the following code to help you out.
```html
<body>
    <button onclick="trythis()">Press me!</button>  <!-- we have a button that calls a function called trythis() -->
    <script src="scripts.js"></script>
</body>
```
```js
let trythis = () => {

    /* 
        This is an empty function, whatever code 
        is placed in here is called when the button is clicked.
    */
}
```
Number Conversions
-
Javascript makes use of the functions parseInt(string) and parseFloat(string) to get a number value from a string. The functions can be linked to a variable so that the numbers can be used in calculations etc.
```js
var input1 = "32"; //this is a string
var number1 = parseint(input1); //this is now a number
```
Just some applications:
```js
alert("Welcome to the KM and Miles Converter!")

var MILES = "MILES"
var KM = "KM"
var userinput = prompt("Please Enter KM to convert KM to miles or enter MILES to convert miles to KM", "ENTER");

if (userinput === KM) {
    var userinput1 = prompt("Enter how many KM you want to convert to miles!")
    var answer = userinput1 * 0.62137119

    alert("The miles are " + answer)

} else if (userinput = MILES) {
    var userinput2 = prompt("Please enter the amount of miles")
    var answer2 = userinput2 * 1.609344

    alert("The kilometres are " + answer2)
}

let txt;

let keepgoing = true;
let NO = "n";
do {


    let response = prompt("I am going to get a drink soon! Do you want me to keep going? y/n")

    if (response === NO) {
        keepgoing = false
    }



} while (keepgoing == true);
console.log(txt);
```
That was a miles to KM converter on JavaScript.

Console App C#:
```C#
bool keepgoing = true;
            do
            {

                Console.WriteLine("Welcome to the Metric System Conversion 2.0");
                Console.WriteLine("");
                Console.WriteLine("Enter the code for what you want to convert");
                Console.WriteLine("");
                Console.WriteLine("Pounds to Kilograms           Code: PTK");
                Console.WriteLine("Inches to Centremeters        Code: ITC");
                Console.WriteLine("Yards to Meters               Code: YTM");
                Console.WriteLine("Miles to Kilometres           Code: MTK");
                Console.WriteLine("Centimetres to Feet/Foot      Code: CTF");
                Console.WriteLine("Feet to Centimetres           Code: FTC");
                Console.WriteLine("Kilograms to Pounds           Code: KTP");
                Console.WriteLine("");
                Console.WriteLine("WANT TO QUIT? JUST TYPE IN THIS CODE       Code: Q");
				Console.WriteLine("");
                Console.Write("Enter Code:");

                String UserInput = Console.ReadLine();
                String PTK = "PTK";
                String ITC = "ITC";
                String YTM = "YTM";
                String MTK = "MTK";
                String QUIT = "Q";
                String CTF = "CTF";
                String FTC = "FTC";
                String KTP = "KTP";


                if (UserInput == PTK)
                {


                    Console.WriteLine("Enter the number of pounds to convert to Kilograms:");
                    double number = double.Parse(Console.ReadLine());
                    double convertedNumber = Math.Round(number / 2.2046, 2);
					Console.WriteLine("");
                    Console.WriteLine($"{convertedNumber}KG");
					Console.WriteLine("");
                    Console.WriteLine("PRESS ENTER TO DO ANOTHER CALCULATION OR PRESS ENTER THEN TYPE Q TO QUIT THE APP");
                    Console.ReadLine();
                }
                else if (UserInput == KTP)
                {
					Console.WriteLine("Enter the number of Kilograms to convert to Pounds:");
					double number = double.Parse(Console.ReadLine());
					double convertedNumber = Math.Round(number * 2.2046, 2);
					Console.WriteLine("");
					Console.WriteLine($"{convertedNumber}lb");
					Console.WriteLine("");
					Console.WriteLine("PRESS ENTER TO DO ANOTHER CALCULATION OR PRESS ENTER THEN TYPE Q TO QUIT THE APP");
					Console.ReadLine(); 
                }
                else if (UserInput == ITC)
                {


                    Console.WriteLine("ENTER THE NUMBER OF INCHES TO CONVERT TO CENTREMETRES:");
                    double number = double.Parse(Console.ReadLine());
                    double convertedNumber = Math.Round(number * 2.54, 2);
					Console.WriteLine("");
                    Console.WriteLine($"{convertedNumber}CM");
					Console.WriteLine("");
                    Console.WriteLine("PRESS ENTER TO DO ANOTHER CALCULATION OR PRESS ENTER THEN TYPE Q TO QUIT THE APP");
                    Console.ReadLine();
                }
                else if (UserInput == QUIT)
                {
                    keepgoing = false;
                    Console.WriteLine("THANK YOU FOR THE METRIC SYSTEM 2.0 APPLICATION PRESS ENTER TO CLOSE");
                }
                else if (UserInput == FTC)
                {
                    Console.WriteLine("ENTER THE NUMBER OF FEET TO CONVERT TO CENTIMETRES");
                    double number = double.Parse(Console.ReadLine());
                    double covertedNumber = Math.Round(number / 0.0328084, 1);
                    Console.WriteLine("");
                    Console.WriteLine($"{covertedNumber}'");
                    Console.WriteLine("");
					Console.WriteLine("PRESS ENTER TO DO ANOTHER CALCULATION OR PRESS ENTER THEN TYPE Q TO QUIT THE APP");
					Console.ReadLine();
                }
                else if (UserInput == CTF)
                {
                    Console.WriteLine("ENTER THE NUMBER OF CENTIMETRES TO FEET");
                    double number = double.Parse(Console.ReadLine());
                    double convertedNumber = Math.Round(number * 0.0328084, 1);
                    Console.WriteLine("");
                    Console.WriteLine($"{convertedNumber}'");
                    Console.WriteLine("");
                    Console.WriteLine("PRESS ENTER TO DO ANOTHER CALCULATION OR PRESS ENTER THEN TYPE Q TO QUIT THE APP");
                    Console.ReadLine();
                }
                else if (UserInput == YTM)
                {
                    Console.WriteLine("ENTER THE NUMBER OF YARDS TO CONVERT TO METRES:");
                    double number = double.Parse(Console.ReadLine());
                    double convertedNumber = Math.Round(number * 0.9144, 2);
					Console.WriteLine("");
                    Console.WriteLine($"{convertedNumber}M");
					Console.WriteLine("");
                    Console.WriteLine("PRESS ENTER TO DO ANOTHER CALCULATION OR PRESS ENTER THEN TYPE Q TO QUIT THE APP");
                    Console.ReadLine();
                }
                else if (UserInput == MTK)
                {
                    Console.WriteLine("ENTER THE NUMBER OF MILES TO KILOMETRES:");
                    double number = double.Parse(Console.ReadLine());
                    double convertedNumber = Math.Round(number * 1.60934, 2);
                    Console.WriteLine("");
                    Console.WriteLine($"{convertedNumber}KM");
                    Console.WriteLine("");
                    Console.WriteLine("PRESS ENTER TO DO ANOTHER CALCULATION OR PRESS ENTER THEN TYPE Q TO QUIT THE APP");
                    Console.ReadLine();
                }
                else
                {
                    Console.WriteLine("");
                    Console.WriteLine("INCORRECT CODE!");
                    Console.WriteLine("");

                }

            }
            while (keepgoing == true);
            {
                Console.ReadLine();
            }
```
# Fruits APPLICATION C#
```js
using System;
using System.Collections.Generic;
namespace Task3
{
    class Program
    {
        static void Main(string[] args)
        {
            //Clear Console to set anew
            Console.Clear();
            //Create var
            var Fruits = new string[5];
            var count = 5;
            //string[] step = {"1st", "2nd", "3rd", "4th", "5th"};
            
            //Create for loop 
            for (var i = 0; i < count; i++)
            {
            
                //string value = step[];
              
            //Ask for a Fruit
            Console.WriteLine($"Type in a Fruit");
                
            //User input
            Fruits[i] = Console.ReadLine();
            //Inform user of data input
           Console.WriteLine($"You picked {Fruits[i]}");
           Console.WriteLine();
            }

            //Print in Ascending Order
            Array.Sort(Fruits);
            Console.WriteLine($"In Order you picked {string.Join(",",Fruits)}");

            //Print in Descending Order.
            Array.Reverse(Fruits);
            Console.WriteLine($"Reverse Order is {String.Join(",", Fruits)}");

            //Close program
            Console.ReadKey();
        }
    }
}
```
# JavaScriopt Application
```js
var fruit = [];
for (let i = 0; i < 5; i++) {
    fruit.push(prompt("Please enter a fruit:"))
}
var fruitjoin = fruit.sort(', ');
var fruitreverse = fruit.reverse(', ');
alert("This is the fruit in asending order " + fruitjoin);
Alert("This is the fruit in desending order " + fruitreverse);
```
>C# Average program
```
using System;

namespace problem2
{
    class Program
    {
        static void Main(string[] args)
        {
            //Start the program with Clear();
            Console.Clear();
            
            Console.WriteLine("Welcome to the number application");

            var number = 0;
            var counter = 10;

            for (var i = 0; i < counter; i++)
            {
                Console.WriteLine("Please enter a number:");
                var isNumber = int.TryParse(Console.ReadLine(), out int input);

                number += input;
            }
            System.Console.WriteLine();
            Console.WriteLine($"The total number is {number}");
            System.Console.WriteLine();
            System.Console.WriteLine($"The average is {number / counter}");
            Console.ReadLine();

             //End the program with blank line and instructions
            Console.ResetColor();
            Console.WriteLine();
            Console.WriteLine("Press <Enter> to quit the program");
            Console.ReadKey();
        }
    }
}
```


>JavaScript Average APPLICATION
```js
let number = 0
let counter = 10

for (let i = 0; i < counter; i++) {

    let answer = prompt("Please type in a number", "")

    number += parseInt(answer)
}

console.log("The total number is = " + number);
console.log("The average of the total = " + number / counter);
```
C# APP
```c#
 //Start the program with Clear();
            Console.Clear();
            
            
            
            bool keepgoing = true;

            do {
            var number = 0;

            Console.WriteLine("Please type in a number:");

            var isNumber = int.TryParse(Console.ReadLine(), out number);

            if(isNumber) 
            {
                keepgoing = false;
                Console.WriteLine($"The number is {number}");
                 //End the program with blank line and instructions
            Console.ResetColor();
            Console.WriteLine();
            Console.WriteLine("Press <Enter> to quit the program");
            Console.ReadKey();
            }
            }
            while (keepgoing == true);
            {
                Console.WriteLine("You didn't enter a number");
            }
            ```
            
            >C# Average APP
            ```c#
             //Start the program with Clear();
            Console.Clear();
            
            Console.WriteLine("Welcome to the number application");

            var number = 0;
            var counter = 10;

            for (var i = 0; i < counter; i++)
            {
                Console.WriteLine("Please enter a number:");
                var isNumber = int.TryParse(Console.ReadLine(), out int input);

                number += input;
            }
            System.Console.WriteLine();
            Console.WriteLine($"The total number is {number}");
            System.Console.WriteLine();
            System.Console.WriteLine($"The average is {number / counter}");
            Console.ReadLine();

             //End the program with blank line and instructions
            Console.ResetColor();
            Console.WriteLine();
            Console.WriteLine("Press <Enter> to quit the program");
            Console.ReadKey();
 ```
# Monday Test Notes (Apart for GitHub)

Random Numbers 

```c

using System;
using System.Collections.Generic;

namespace Random_Number_Csharp
{
    class Program
    {
        static List<string> cars = new List<string> { "Audi", "Mazda", "Toyota", "Nissan" };
        static List<string> drivers = new List<string> { "Bob", "Lisa", "Tim", "Simon", "Kevin" };
        static void Main(string[] args)
        {
            //Start the program with Clear();
            Console.Clear();

            Console.WriteLine(DisplayDriver());
            Console.WriteLine(DisplayDriver());
            Console.WriteLine(DisplayDriver());

            //End the program with blank line and instructions
            Console.ResetColor();
            Console.WriteLine();
            Console.WriteLine("Press <Enter> to quit the program");
            Console.ReadKey();
        }

        static int GenerateRandomNumber(List<string> myList)
        {
            var rand = new Random();
            return rand.Next(1, myList.Count);
        }

        static string DisplayDriver()
        {

            var selectedCar = cars[GenerateRandomNumber(cars)];
            var selectedDriver = drivers[GenerateRandomNumber(drivers)];

            //return $"{selectedDriver} is driving the {selectedCar}";
            return $"Selected Driver = {selectedDriver}\nSelected Car = {selectedCar}";
        }
    }
}
```

Classes

```C
using System;

namespace Create_Classes
{
    class cars
    {
        private string _Make;

        private string _Model;

        private int _Year;

        public string Make
        {

            set
            {
                _Make = value;

            }
        }

        public string Model
        {

            set
            {
                _Model = value;

            }
        }

        public int Year
        {

            set
            {
                _Year = value;

            }
        }

        public cars(string _make, string _model, int _year)
        {
            Make = _make;
            Model = _model;
            Year = _year;
        }

        public string DisplayCar()
        {
            var showmycar = "The car we have created is: \n\n";
            showmycar += $"The Make is {_Make}\n";
            showmycar += $"The Model is {_Model}\n";
            showmycar += $"The Year is {_Year}\n";

            return showmycar;
        }
    }

    class Program
    {
        static void Main(string[] args)
        {
            var car1 = new cars("Mazda", "RX7", 1974);
            var car2 = new cars("Mercedes-Benz", "AMG", 2011);
            var car3 = new cars("Ford", "Model T", 1914);
        }
    }
}
```
Methods
```c
using System;
using System.Collections.Generic;

namespace Methods
{
    class Program
    {
        static void Main(string[] args)
        {
            //PrintToScreen();
            //PrintNameWithParam("Jeff");
            //PrintNameWithParam("Bob");
            //PrintNameWithParam("Tim");

            //PrintStringUsingParam("Hello my name is fuck you");

            //var greeting = Greeting("Dayne");

            Console.WriteLine(Calculate(2, 3, "/"));
        }

        static void PrintToScreen(){
            Console.WriteLine("Hello my name is Dayne Game");
        }

        static void PrintNameWithParam(string name) {
            Console.WriteLine($"Hello my name is {name}");
        }

        static void PrintStringUsingParam(string content) {
            Console.WriteLine($"  {content}");
        }

        static string Greeting(string name) {

            return $"hello my name is {name}";

        }

        static string Calculate(double num1, double num2, string op) {

            var answer = string.Empty;

            switch(op) {

                case("*"):
                    answer = $"{num1} x {num2} = {num1 * num2}";
                break;

                case("+"):
                    answer = $"{num1} + {num2} = {num1 + num2}";
                break;

                case("/"):
                    answer = $"{num1} / {num2} = {num1 / num2}";
                break;

                case("-"):
                    answer = $"{num1} - {num2} = {num1 - num2}";
                break;

                default:
                    answer = "You entered an invalid operator";
                break;

            }
            
            
            
            return answer;
        }
    }
}
```         
     