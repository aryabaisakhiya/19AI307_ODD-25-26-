# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
In a haunted house, lights turn on or off based on the hour of entry:

If the hour is even and between 2 and 6 (inclusive), lights flicker.

If the hour is odd and between 7 and 11, lights stay off.

If the hour is 12, lights turn red.

Otherwise, the house is dark.

The program will print one of the following statements based on the input:

Lights flicker

Lights off

Lights red

Dark house


## AIM:
To create a Java program that takes an hour as input and displays the haunted house light status based on given conditions.


## ALGORITHM :
1.Start

2.Read the hour value

3.If hour is even and between 2 and 6 → print "Lights flicker"

4.Else if hour is odd and between 7 and 11 → print "Lights off"

5.Else if hour is 12 → print "Lights red"

6.Else → print "Dark house"

7.End


## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: Arya Baisakhiya
RegisterNumber: 212222040019
*/
```

## SOURCE CODE:
```
import java.util.*;

public class HauntedHouse {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int hour = sc.nextInt();

        if (hour % 2 == 0 && hour >= 2 && hour <= 6) {
            System.out.println("Lights flicker");
        } else if (hour % 2 != 0 && hour >= 7 && hour <= 11) {
            System.out.println("Lights off");
        } else if (hour == 12) {
            System.out.println("Lights red");
        } else {
            System.out.println("Dark house");
        }

        sc.close();
    }
}
```

## OUTPUT:
<img width="456" height="298" alt="image" src="https://github.com/user-attachments/assets/e66d2bb5-3d21-4286-9ba6-475f95cb5ead" />




## RESULT:
The program was implemented successfully and verified.

