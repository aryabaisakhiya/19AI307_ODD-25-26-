# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Write a Java program to convert a string to an integer using a wrapper class and perform addition.

## AIM:
To develop a Java program that converts a numeric string into an integer using a wrapper class (Integer.parseInt()) and performs addition.

## ALGORITHM :
```
1.Start
2.Read a numeric string from the user
3.Convert the string to an integer using Integer.parseInt()
4.Read another integer value and add it to the converted number
5.Display the result of the addition and end
```
## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: Arya Baisakhiya
RegisterNumber: 212222040019
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        String input1=sc.nextLine();
        String input2=sc.nextLine();
        int num1=Integer.parseInt(input1);
        int num2=Integer.parseInt(input2);
        int sum=num1+num2;
        System.out.println("Sum = "+sum);
    }
}
```

## OUTPUT:
<img width="323" height="282" alt="image" src="https://github.com/user-attachments/assets/90d99378-f819-42d1-bdbd-892e60997539" />

## RESULT:
The program was implemented successfully and verified.



