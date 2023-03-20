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
```C#
using System;
namespace palindrome
{
    public class program
    {
        public static void Main(string[] args)
        {
            string str,rev;
            int i;
            rev = string.Empty;
            Console.WriteLine("Enter the string:");
            str= Console.ReadLine();
            for(i=str.Length-1;i>=0;i--)
            {
                rev += str[i].ToString();
            }
            if (rev == str)
            {
                Console.WriteLine(str+" aPalindrome");
            }
            else
            {
                Console.WriteLine(str+" Not Palindrome");
            }
        }
    }
}
```
## Output:
![ss1](./ss1.png)
![ss2](./ss2.png)
## Result:
Thus the C# program to display whether the given string is Palindrome or not is executed successfully.
