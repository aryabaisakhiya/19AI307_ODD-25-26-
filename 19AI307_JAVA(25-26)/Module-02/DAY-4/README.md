# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write Java code to create a class Triangle and initialiaze the attributes(base and height) using default constructor and calculate the area of the triangle using user defined function.


## AIM:
To write a Java program to  create a class Triangle and initialiaze the attributes(base and height) using default constructor and calculate the area of the triangle.

## ALGORITHM :
```
1. Start
2. Create a class named **Triangle**
3. Declare attributes **base** and **height**
4. Use a **default constructor** to initialize base and height with fixed values
5. Calculate area using `area = 0.5 * base * height` and display it, then end
```

## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: Arya Baisakhiya 
RegisterNumber: 212222040019  
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class prog {
    double base, height;

    prog() {
        Scanner sc = new Scanner(System.in);
        base = sc.nextDouble();
        height = sc.nextDouble();
    }

    void calculateArea() {
        double area = (base * height) / 2;
        System.out.println("Area of the triangle is: " + area);
    }

    public static void main(String[] args) {
        prog t = new prog();
        t.calculateArea();
    }
}
```

## OUTPUT:
<img width="727" height="315" alt="image" src="https://github.com/user-attachments/assets/8aac7d8c-7a06-404b-a2fb-28a85e03b2b4" />




## RESULT:
The program was implemented successfully and verified.


