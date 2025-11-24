# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Define class Game with: Static variable maxScore = 500 Print max score via 3 different object references. Change via one object into 800, and print the output of previous maxScore and changed maxScore. 

## AIM:
To write a Java program to create a class Game with a static variable maxScore and demonstrate how static data is shared among all objects by modifying it through one object and printing the results.


## ALGORITHM :
```
1.Start
2.Create a class Game with a static variable maxScore = 500
3.Create three objects of the Game class and print maxScore using each object
4.Modify maxScore to 800 using one object
5.Print the previous and updated maxScore values to show the change, then end
```

## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: Arya Baisakhiya
RegisterNumber: 212222040019
*/
```

## SOURCE CODE:
```
class Game{
    static int maxScore = 500;
}
class prog{
    public static void main(String[] args){
        Game g1 = new Game();
        Game g2 = new Game();
        Game g3 = new Game();
        System.out.println(g1.maxScore);
        System.out.println(g2.maxScore);
        System.out.println(g3.maxScore);

        g1.maxScore = 800;
        System.out.println(g1.maxScore);
        System.out.println(g1.maxScore);
        System.out.println(g1.maxScore);


                
    }
}
```
## OUTPUT:
<img width="253" height="280" alt="image" src="https://github.com/user-attachments/assets/9b568e0e-dc76-4108-8e9a-2560237d56af" />

## RESULT:
The program was implemented successfully and verified.


