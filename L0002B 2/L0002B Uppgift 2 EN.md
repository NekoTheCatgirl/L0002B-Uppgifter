# Classes, Lists, Sorting and Files
In this assignment you will be creating classes, using lists, sorting data, and writing files.

This may be done either as a Console Application or a Windows Forms Application <br>
![Console Application](Images/ConsoleApplication.png) <br>
![Windows Forms Application](Images/WindowsFormsApplication.png) <br>

## What you will need to do
You will create a application that takes in "Name", "Social security number", "District", "Amount of sold articles", add it to a list, then writing out the list to a file. 

`Seller` Has the information that was given `(name, social security number, district and amount)`

When you write the infomation you will have to think about that there are 4 levels for the sellers, `bellow 50 articles`, `50-99 articles`, `100-199 articles`, `over 199 articles`

Sort your list of `Seller` based on `Amount of sold articles` and then write it out like the example bellow:
```
Namn        Persnr      Distrikt        Antal
Kalle Anka  4503038990  Piteå           173
1 säljare har nått nivå 3: 100-199 artiklar

Musse Pigg  3502038964  Boden           202
Snobben     7805055673  Luleå           203
2 säljare har nått nivå 4: över 199 artikla
```
Etc...
## Some helpfull tips
- Utilize standard libraries, Linq is great for lists
```cs
List<int> numbers = new List<int>() {
    5,
    0,
    69,
    74,
    35,
    86
};

numbers.Sort((first, second) => first.CompareTo(second));
/*
The list is now in this order instead:
0,
5,
35,
69,
74,
86
*/
```
- You can override functions on your classes
```cs
class MyClass {
    public int value;

    public override string ToString() {
        return "The value is " + value;
    }
}

MyClass my_object = new MyClass() {
    value = 69
};

// This will write out "The value is 69"
Console.WriteLine(my_object.ToString());
```
- Utilize the right loop for the job
```cs
// Do work on a range of numbers
for (int i = 0; i < 50; i++) {
    Console.WriteLine(i);
}

// Iterate over a collection
List<int> numbers = new List<int>() {
    5,
    0,
    69,
    74,
    35,
    86
};
foreach (int number in numbers) {
    Console.WriteLine(number);
}

// Do work until a condition is met
int number = 0;
while (number == 0) {
    Console.WriteLine("Write a number");
    string input = Console.ReadLine()
    try {
        number = int.Parse(input);
    }
    catch (FormatException) {
        Console.WriteLine("That was not a number, try again");
    }
}
Console.WriteLine("Your number is " + number);
```
- When writing files, you do not have to specify the whole path
```cs
// This is a relative path, so will take the working directory, and try to write a file in it with the name "file.txt"
File.WriteAllText("file.txt", "Hello from C#!");
```

## Turning in your assignment
You will need to zip up the whole project into a zip archive

For winrar you can follow these steps: <br>
![Winrar 1](Images/Winrar1.png) <br>
Then <br>
![Winrar 2](Images/Winrar2.png) <br>