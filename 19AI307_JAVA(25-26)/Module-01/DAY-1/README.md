# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:
Lovely wants to enter a secure tech conference. The security system checks certain conditions to grant access. These conditions are:

She must be registered (true/false).

She must have a valid ID (true/false).

She must NOT be blacklisted (true/false).

The system uses logical operators to evaluate her access eligibility:

If she is registered AND has a valid ID, and NOT blacklisted, she is granted access.

Otherwise, access is denied.

Your task is to evaluate these conditions using logical operators and print whether access is granted or denied.

## AIM:
To write a program to evaluate the conditions using logical operators and print whether access is granted or denied.



## ALGORITHM :
1. Start the program and create a Scanner object.
2. Read the three boolean inputs.
3. Evaluate the condition: registered AND valid ID AND NOT blacklisted.
4. Store the result in `accessGranted`.
5. Print whether access is granted.



## PROGRAM:
 ```
/*
Program to implement variables and Operators using Java
Developed by: Arya Baisakhiya   
RegisterNumber: 212222040019  
*/
```

## Sourcecode.java:

import java.util.Scanner;

public class AccessCheck {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        boolean isRegistered = sc.nextBoolean();
        boolean hasValidID = sc.nextBoolean();
        boolean isBlacklisted = sc.nextBoolean();
        boolean accessGranted = (isRegistered && hasValidID && !isBlacklisted);
        System.out.println("Access Granted: " + accessGranted);
    }
}










## OUTPUT:

![Uploading image.png…]()




## RESULT:

