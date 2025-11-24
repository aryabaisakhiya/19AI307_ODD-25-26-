# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Create a class Vehicle with attributes as number, type and owner.

## AIM:
To write a Java program to create a class Vehicle with attributes as number, type and owner.

## ALGORITHM :
```
1.Start
2.Define a class named Vehicle
3.Inside the class, declare attributes: number, type, and owner
4.Create a constructor to initialize these attributes
5.Create a method to display the vehicle details and end
```
## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by:Arya Baisakhiya 
RegisterNumber: 212222040019
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
class Vehicle{
    String number;
    String type;
    String owner;
}
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Vehicle v1 = new Vehicle();
        v1.number = sc.next();
        v1.type = sc.next();
        v1.owner = sc.next();

        Vehicle v2 = new Vehicle();
        v2.number = sc.next();
        v2.type = sc.next();
        v2.owner = sc.next();

        System.out.println(v1.number + " | " + v1.type + " | " + v1.owner);
        System.out.println(v2.number + " | " + v2.type + " | " + v2.owner);

        sc.close();
    }
}

```
## OUTPUT:
<img width="792" height="248" alt="image" src="https://github.com/user-attachments/assets/431fd37e-8566-434c-8241-7423591cac54" />




## RESULT:
The program was implemented successfully and verified.

