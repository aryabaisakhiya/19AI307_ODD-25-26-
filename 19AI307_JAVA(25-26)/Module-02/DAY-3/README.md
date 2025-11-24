# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to create a class called BankAccount with private instance variables accountNumber and balance. Provide public getter and setter methods to access and modify these variables.

## AIM:
To write a Java program to  create a class called BankAccount with private instance variables accountNumber and balance.


## ALGORITHM :
```
1. Start
2. Create a class named BankAccount
3. Declare private instance variables: accountNumber and balance
4. Write a constructor to initialize these variables
5. Provide public methods (getters/setters or deposit/withdraw) to access and modify the balance, then end
```
## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: Arya Baisakhiya
RegisterNumber: 212222040019  
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class BankAccount {
    private String accountNumber;
    private double balance;

    public String getAccountNumber() {
        return accountNumber;
    }
    public void setAccountNumber(String accountNumber) {
        this.accountNumber = accountNumber;
    }

    public double getBalance() {
        return balance;
    }
    public void setBalance(double balance) {
        this.balance = balance;
    }
}

public class prog {
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        
        BankAccount b1 = new BankAccount();
        
     
        String a = scan.nextLine();
        double b = scan.nextDouble();

        b1.setAccountNumber(a);
        b1.setBalance(b);
        
        System.out.println("Account Number: " + b1.getAccountNumber());
        System.out.println("Balance: " + b1.getBalance());
        
        
    }
}

```
## OUTPUT:
<img width="781" height="378" alt="image" src="https://github.com/user-attachments/assets/1fe23e52-2544-4db7-9e21-40397b9a505c" />




## RESULT:
The program was implemented successfully and verified.



