# Palindrome


## Aim:
To write a C# program to find whether the given string is a Palindrome or not.
## Algorithm:
### Step 1:
Create a new Class named palindrom.

### Step 2:
Declare three variables of string data type.

input - Store the input from user.
str - Convert user input to lower case and store it.
pal - Reverse the string str and store it.
### Step 3:
Get input from the user and store it. Then convert it to lower case.

### Step 4:
Using for loop, iterate through the each character from the end to begining and add it to the new variable called pal

### Step 5:
Using If-else statement check whether the input string & reversed string are same.

### Step 6:
Print the input and reversed string along with the whether palindrom or not.

### Step 7:
End of the Program.

## Program:
```
using System;
namespace palindrome
{
    class Program
    {
        static void Main(string[] args)
        {
            string s, revs = "";
            Console.WriteLine(" Enter string");
            s = Console.ReadLine();
            for (int i = s.Length - 1; i >= 0; i--)  
            {
                revs += s[i].ToString();
            }
            if (revs == s) 
            {
                Console.WriteLine("String is Palindrome \nEntered String: {0}\nReverse string: {1}", s, revs);
            }
            else
            {
                Console.WriteLine("String is not Palindrome \n Entered String: {0}\nReverse string: {1}", s, revs);
            }
            Console.ReadKey();
        }
    }
}
```

## Output:
![o](cc1.png)
![o](cc2.png)

## Result:
Thus the C# program to display whether the given string is Palindrome or not is executed successfully.
