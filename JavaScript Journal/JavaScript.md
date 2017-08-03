JavaScript Journal

How to add files to github
1. cd desktop
2. git init (name of folder without brackets)
3. cd (name of folder created)
4. code .
5. Then create a file called index.html and script.js
6. Use ctrl ` (backtick) to open the intergrated terminial

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

>*This is how you link your javascript file with your HTML:
```
 <script src="script.js"></script>
 ```

How to make a variable:
```
var a = "This is the value"
```

How to make a constant (constants cannot be changed)
```
const a = "This is the value"
```
How to do a varaible scope:
```
var a = 10;

if (a <= 10 )
{
    var b = 10;
    a += b;
    document.WriteLine("The new value of a = " + a)
}

document.writeLine("The value for variable a is now "+ a) //This will return a value
document.writeLine("The value for variable b is now "+ b) //This will also work
```

Variable scope using let instead of var:
```
let a = 10;

if (a <= 10 )
{
    let b = 10;
    a += b;
    document.WriteLine("The new value of a = " + a)
}

document.writeLine("The value for variable a is now "+ a) //This will return a value
document.writeLine("The value for variable b is now "+ b) //This will no longer work
```