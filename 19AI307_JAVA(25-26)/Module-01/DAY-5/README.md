# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to reverse a given string.

## AIM:
To create a Java program to reverse a given string.


## ALGORITHM :
```
1.Start
2.Read the input string
3.Initialize an empty string rev
4.Traverse the original string from end to start and append each character to rev
5.Display rev and end
```
## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
Developed by: Arya Baisakhiya
RegisterNumber: 212222040019  
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class ReverseString {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String input = sc.nextLine();
        String reversed = "";
        for (int i = input.length() - 1; i >= 0; i--) {
            reversed += input.charAt(i);
        }
        System.out.println("Reversed string: " + reversed);
        
    }
}

```
## OUTPUT:
<img width="647" height="252" alt="image" src="https://github.com/user-attachments/assets/675e27ac-2b76-462c-b353-40e3bd446c8d" />




## RESULT:
The program was implemented successfully and verified.

