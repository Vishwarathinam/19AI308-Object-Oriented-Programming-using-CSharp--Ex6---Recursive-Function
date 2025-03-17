# 19AI308-Object-Oriented-Programming-using-CSharp--Ex6---Recursive-Function
## Aim: 
To write a C# program to reverse a number using a recursive function.

## Algorithm:
### Step 1:
Create a class called reverse.

### Step 2:
Create a recursive function named RevNum to reverse the number

### Step 3:
In the function find a reminder of the number multiply it by 10 and add the reverse number.

### Step 4:
Recursively call this function to get the reversed number.

### Step 5:
Create a Main function

### Step 6:
Get input from the user for the number to be reversed.

### Step 7:
Call the function RevNum

### Step 8:
End of the program.

## Program:
```cs
using System;

public class reverse
{
    static int RevNum(int n, int rev = 0)
    {
        if (n == 0)
        {
            return rev;
        }
        int digit = n % 10;
        rev = rev * 10 + digit;
        return RevNum(n / 10, rev);
    }

    static void Main(string[] args)
    {
        Console.Write("Enter a number to reverse: ");
        int number = Convert.ToInt32(Console.ReadLine());
        Console.WriteLine("Reversed number: {0}", RevNum(number));
    }
}
```

## Output:
![](https://github.com/Ronick2005/19AI308-Object-Oriented-Programming-using-CSharp--Ex6---Recursive-Function/assets/83219341/df78ed04-89ce-46bb-afbd-9b249d0e68d0)

## Result:
Thus C# program to reverse a number using recursive function is written and executed sucessfully.
