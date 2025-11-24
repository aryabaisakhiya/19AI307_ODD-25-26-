# Ex.No:3(A) INHERITANCE AND AGGREGATION

## QUESTION:
A jewelry store tracks gold rates for different types of customers. The base class is Customer with attributes like customerId, name, and purchaseWeight (in grams). There are two types of customers: RegularCustomer and PremiumCustomer. RegularCustomer gets a fixed discount of 2% on the gold rate per gram. PremiumCustomer gets a 5% discount plus a special cashback. The base gold rate per gram is input at runtime. For each customer, calculate the final price they pay:
finalPrice = purchaseWeight * (goldRatePerGram - discount)
For PremiumCustomer, additionally show cashback amount (which is 1% of the final price).

## AIM:
To develop an inheritance-based program with a Customer base class and two derived classes, RegularCustomer and PremiumCustomer, to calculate the final price of gold purchases based on discounts and cashback, using the gold rate entered at runtime.


## ALGORITHM :
```
1.Start
2.Read the gold rate per gram from the user
3.Create the base class Customer with attributes: customerId, name, and purchaseWeight
4.Create RegularCustomer class that applies a 2% discount on the gold rate per gram
5.Create PremiumCustomer class that applies a 5% discount and calculates 1% cashback on the final price
6.For each customer, compute
finalPrice = purchaseWeight × (goldRatePerGram − discount)
Display final price; for PremiumCustomer, also display cashback; then end
```
## PROGRAM:
 ```
/*
Program to implement a Inheritance and Aggregation using Java
Developed by:Arya Baisakhiya 
RegisterNumber: 212222040019 
*/
```

## SOURCE CODE:
```

import java.util.Scanner;
import java.text.DecimalFormat;

class Customer {
    String customerId, name;
    double purchaseWeight, goldRatePerGram;

    Customer(String customerId, String name, double purchaseWeight, double goldRatePerGram) {
        this.customerId = customerId;
        this.name = name;
        this.purchaseWeight = purchaseWeight;
        this.goldRatePerGram = goldRatePerGram;
    }

    double getDiscountRate() {
        return 0;
    }

    double calculateFinalPrice() {
        double discountAmount = goldRatePerGram * getDiscountRate() / 100;
        double effectiveRate = goldRatePerGram - discountAmount;
        return purchaseWeight * effectiveRate;
    }

    void display() {
        DecimalFormat df = new DecimalFormat("0.00");
        System.out.println("Customer ID: " + customerId);
        System.out.println("Name: " + name);
        System.out.println("Customer Type: General");
        System.out.println("Purchase Weight: " + purchaseWeight + " grams");
        System.out.println("Gold Rate per Gram: " + goldRatePerGram);
        System.out.println("Discount: " + getDiscountRate() + "%");
        System.out.println("Final Price: " + df.format(calculateFinalPrice()));
    }
}

// Regular Customer
class RegularCustomer extends Customer {
    RegularCustomer(String customerId, String name, double purchaseWeight, double goldRatePerGram) {
        super(customerId, name, purchaseWeight, goldRatePerGram);
    }

    @Override
    double getDiscountRate() {
        return 2;
    }

    @Override
    void display() {
        DecimalFormat df = new DecimalFormat("0.00");
        System.out.println("Customer ID: " + customerId);
        System.out.println("Name: " + name);
        System.out.println("Customer Type: Regular");
        System.out.println("Purchase Weight: " + purchaseWeight + " grams");
        System.out.println("Gold Rate per Gram: " + goldRatePerGram);
        System.out.println("Discount: " + (int)getDiscountRate() + "%");
        System.out.println("Final Price: " + df.format(calculateFinalPrice()));
    }
}

// Premium Customer
class PremiumCustomer extends Customer {
    PremiumCustomer(String customerId, String name, double purchaseWeight, double goldRatePerGram) {
        super(customerId, name, purchaseWeight, goldRatePerGram);
    }

    @Override
    double getDiscountRate() {
        return 5;
    }

    double calculateCashback() {
        return calculateFinalPrice() * 0.01;
    }

    @Override
    void display() {
        DecimalFormat df = new DecimalFormat("0.00");
        System.out.println("Customer ID: " + customerId);
        System.out.println("Name: " + name);
        System.out.println("Customer Type: Premium");
        System.out.println("Purchase Weight: " + purchaseWeight + " grams");
        System.out.println("Gold Rate per Gram: " + goldRatePerGram);
        System.out.println("Discount: " + (int)getDiscountRate() + "%");
        System.out.println("Final Price: " + df.format(calculateFinalPrice()));
        System.out.println("Cashback: " + df.format(calculateCashback()));
    }
}

// Main Driver
public class JewelryStore {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);


while (sc.hasNextLine()) {
    String customerType = sc.nextLine().trim();
    if (customerType.isEmpty()) break; 

    String customerId = sc.nextLine().trim();
    String name = sc.nextLine().trim();
    double purchaseWeight = Double.parseDouble(sc.nextLine().trim());
    double goldRatePerGram = Double.parseDouble(sc.nextLine().trim());

    Customer c;
    if (customerType.equalsIgnoreCase("Regular")) {
        c = new RegularCustomer(customerId, name, purchaseWeight, goldRatePerGram);
    } else {
        c = new PremiumCustomer(customerId, name, purchaseWeight, goldRatePerGram);
    }

    c.display();
    System.out.println();
}

sc.close();

    }
}


```

## OUTPUT:
<img width="797" height="707" alt="image" src="https://github.com/user-attachments/assets/ba65d9c2-26c0-41c5-8ff1-bcf10c425f2e" />


## RESULT:
The program was implemented successfully and verified.

