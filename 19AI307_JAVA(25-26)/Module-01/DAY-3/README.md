# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
In mathematics, the factorial of a non-negative integer n, denoted as n!, is the product of all positive integers less than or equal to n. For example:

5! = 5 × 4 × 3 × 2 × 1 = 120

3! = 3 × 2 × 1 = 6

0! is defined as 1.

Write a Java program that prompts the user to enter a non-negative integer and then calculates and displays the factorial of the given number.Use a for loop to perform the calculation.Make sure to handle the case when the user enters 0.Display the result in a clear and user-friendly way.

## AIM:
To create a Java program that prompts the user to enter a non-negative integer and then calculates and displays the factorial of the given number.

## ALGORITHM :
1.Start
2.Read a non-negative integer n
3.Initialize fact = 1
4.Loop from 1 to n and multiply each value with fact
5.Display the factorial and end

## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
Developed by: Arya Baisakhiya
RegisterNumber: 212222040019
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        int n = scan.nextInt();

        if (n < 0) {
            System.out.println("Invalid input! Please enter a non-negative integer.");
        } else {
            long factorial = 1;
            for (int i = 1; i <= n; i++) {
                factorial *= i;
            }
            System.out.println("Factorial of " + n + " is: " + factorial);
        }
    }
}
```
## OUTPUT:
<img width="686" height="247" alt="image" src="https://github.com/user-attachments/assets/4a33e790-ee64-4619-89ef-975236620fd7" />

## RESULT:
The program was implemented successfully and verified.

