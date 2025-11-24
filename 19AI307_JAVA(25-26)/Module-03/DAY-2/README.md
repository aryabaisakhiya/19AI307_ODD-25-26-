# Ex.No:3(b) POLYMORPHISM

## QUESTION:
Write a Java program to perform the addition of two numbers using method overloading. The program should contain two overloaded methods named sum():

One that takes two integers and returns their sum.

One that takes two double values and returns their sum.


## AIM:
To write a Java program that demonstrates method overloading by defining two sum() methods—one that adds two integers and another that adds two double values


## ALGORITHM :
```
1.Start
2.Create a class with two overloaded methods sum(): one accepting two integers, another accepting two doubles
3.In each method, return the addition of the given parameters
4.In the main method, call both versions of sum() with integer and double arguments
5.Display the results and end
```
## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: Arya Baisakhiya
RegisterNumber: 212222040019
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class MethodOverloadingSum {

    public static int sum(int a, int b) {
        return a + b;
    }

    public static double sum(double a, double b) {
        return a + b;
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        if (scanner.hasNextInt()) {
            int int1 = scanner.nextInt();
            if (scanner.hasNextInt()) {
                int int2 = scanner.nextInt();
                int intSum = sum(int1, int2);
                System.out.println(intSum);
            }
        }

        if (scanner.hasNextDouble()) {
            double double1 = scanner.nextDouble();
            if (scanner.hasNextDouble()) {
                double double2 = scanner.nextDouble();
                double doubleSum = sum(double1, double2);
                System.out.println(doubleSum);
            }
        }

        scanner.close();
    }
}

```

## OUTPUT:
<img width="315" height="316" alt="image" src="https://github.com/user-attachments/assets/c43975cc-6404-41a7-b946-208ca6b1dc75" />




## RESULT:
The program was implemented successfully and verified.



