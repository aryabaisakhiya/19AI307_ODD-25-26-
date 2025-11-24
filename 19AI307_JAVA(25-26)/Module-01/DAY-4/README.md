# Ex.No:1(D) ARRAYS

## QUESTION:
Write a Java Program to Find the Average of Array Elements.

## AIM:
To create a Java Program to Find the Average of Array Elements.

## ALGORITHM :
```
1.Start
2.Read the number of elements and store them in an array
3.Initialize a variable sum = 0
4.Loop through the array and add each element to sum
5.Compute average = sum / number of elements and display it
6.End
```
## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
Developed by: Arya Baisakhiya
RegisterNumber: 212222040019
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Main{
    public static void main(String[] args){
        Scanner scan=new Scanner(System.in);
        int n=scan.nextInt();
        int[] arr=new int[n];
        int sum=0;
        for(int i=0;i<n;i++){
            arr[i]=scan.nextInt();
            sum+=arr[i];
        }
        double avg=(double)sum/n;
        System.out.printf("The average of elements is %.2f",avg);
    }
}
```
## OUTPUT:
<img width="775" height="486" alt="image" src="https://github.com/user-attachments/assets/62f0a5ca-ae62-46a4-b563-f4d54b6ae656" />

## RESULT:
The program was implemented successfully and verified.




## RESULT:

