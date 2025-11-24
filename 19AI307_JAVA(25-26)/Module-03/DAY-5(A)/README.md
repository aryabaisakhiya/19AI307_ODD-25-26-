# Ex.No:3(E) INNER CLASS

## QUESTION:
Write a Java program to reverse a number using the Integer wrapper class and compare it with the original number.

## AIM:
To write a Java program to check whether a given number is a Palindrome or not using Inner Class.


## ALGORITHM :
```
1.Start
2.Read an integer value from the user
3.Convert the number into a String
4.Reverse the String
5.Convert the reversed String back to integer
6.Compare the original number with reversed number
7.If both are equal, it is a Palindrome
8.Else, it is not a Palindrome
9.Stop
```
## PROGRAM:
 ```
/*
Program to implement a InnerClass using Java
Developed by: Arya Baisakhiya
RegisterNumber: 212222040019  
*/
```

## SOURCE CODE:
```
import java.util.*;
class prog{
    public static void main(String args[])
    {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        String originalStr = Integer.toString(num);
        String reversedStr = new StringBuilder(originalStr).reverse().toString();
        int reversedNum = Integer.parseInt(reversedStr);
        if(num == reversedNum)
        {
            System.out.println(num+" is a palindrome number.");
        }
        else{
            System.out.println(num+" is not a palindrome number.");
            System.out.println("Reversed Number: "+reversedNum);
        }
    }
}
```

## OUTPUT:
<img width="792" height="268" alt="image" src="https://github.com/user-attachments/assets/2b05686d-731b-45f4-9e22-55a0f50197d5" />

## RESULT:
The program was implemented successfully and verified.



