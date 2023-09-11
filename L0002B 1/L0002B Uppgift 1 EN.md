# Operations and Math
This task will go over operations and math.

You will need to do this task using both a Console Application: <br>
![Console Application](Images/ConsoleApplication.png)<br>
And as a Windows Forms Application:<br>
![Windows Forms Application](Images/WindowsFormsApplication.png)<br>

You can make use of .NET Framework or not, does not matter much.

## What you will need to do
You will create a application that takes in 2 numbers, "Cost" and "Payment", and after, return the change from the transaction.

It will be in Swedish currency, bills: `(500, 200, 100, 50, 20)` and coins: `(10, 5, 1)`

Example for given data and expected results:
```
Ange pris: 152      (User gives the Cost)
Betalt: 500         (How much was paid)
Växel tillbaka:
1 tvåhundralapp
1 hundralapp
2 tjugor
1 femkrona
3 enkronor
```

Test your program before turning it in!

## Some helpfull tips
- Create classes that can help you with handeling the many values you will deal with.
```cs
class MyClass {
    // Class values
    int value;

    // Class Constructor
    public MyClass(int number) {
        value = number;
    }

    // Class Function
    public int GetValue() {
        return value;
    }
}
```
- You can assign and modify values after defining
```cs
int my_number;

my_number = 50; // Is now 50
```
- Compound operators are extremely helpfull in minimizing your code
```cs
int my_number = 50;

my_number *= 3; // The value is now 150 as we multiplied it by 3
```
- Break out repetative code into functions
```cs
public string RepetativeFunction(int value) {
    if (value > 0) {
        return "Greater than 0";
    }
    return "Less than or equal to 0";
}
// Imagine this has to be called many times in your code
Console.WriteLine(RepetativeFunction(25));
Console.WriteLine(RepetativeFunction(43));
Console.WriteLine(RepetativeFunction(-125));
Console.WriteLine(RepetativeFunction(263));
Console.WriteLine(RepetativeFunction(0));
Console.WriteLine(RepetativeFunction(53));
Console.WriteLine(RepetativeFunction(-189));
```
## Turning in your assignment
You will need to zip up the whole project into a zip archive

For winrar you can follow these steps:<br>
![Winrar 1](Images/Winrar1.png)<br>
Then <br>
![Winrar 2](Images/Winrar2.png)<br>
