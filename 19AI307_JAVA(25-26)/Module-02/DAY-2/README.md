# Ex.No:2(B) METHODS

## QUESTION:
Write a method int cube(int x) that calls a method int square(int x) internally to calculate the cube as x * square(x).

## AIM:
To create a Java program to write a method int cube(int x) that calls a method int square(int x) internally to calculate the cube of any number. 

## ALGORITHM :
```
1.Start
2.Define a method square(x) that returns x * x
3.Define another method cube(x)
4.Inside cube(x), call square(x) and compute x * square(x)
5.Return the cube value and end
```
## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: Arya Baisakhiya 
RegisterNumber: 212222040019 
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
class prog{
   public int square(int x){
        return x * x;
    }
   public int cube(int x){
        return x * square(x);
    }
    
    public static void main(String[] args){
        prog m1=new prog();
        Scanner scan = new Scanner(System.in);
        int a= scan.nextInt();
        System.out.println(m1.cube(a));
    }
}

```
## OUTPUT:
<img width="311" height="160" alt="image" src="https://github.com/user-attachments/assets/94bd8f74-957b-43ba-a855-a8c163ccff99" />




## RESULT:
The program was implemented successfully and verified.


