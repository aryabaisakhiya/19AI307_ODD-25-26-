# Ex.No:3(C) ABSTRACTION

## QUESTION:
Description:
Create abstract class GameScore with method finalScore().
Subclasses:

ArcadeGame: score = baseScore + (level × 100)

PuzzleGame: score = (attempts ≤ 3) ? 1000 - (attempts × 100) : 500

Input Format:

First line: 1 or 2
Second line: base, level (or attempts)


## AIM:
To develop a Java program using abstraction where an abstract class GameScore defines the method finalScore(), and subclasses ArcadeGame and PuzzleGame compute the final score based on different rules and user inputs.


## ALGORITHM :
```
1.Start
2.Define an abstract class GameScore with an abstract method finalScore()
3.Create ArcadeGame class that calculates score as
score = baseScore + (level × 100)
4.Create PuzzleGame class that calculates score as
score = (attempts ≤ 3) ? 1000 - (attempts × 100) : 500
5.Read the first input (1 for ArcadeGame, 2 for PuzzleGame) and the corresponding values (base & level OR attempts)
6.Create the appropriate object, call finalScore(), display the score, and end
```
## PROGRAM:
 ```
/*
Program to implement a Abstraction using Java
Developed by: Arya Baisakhiya
RegisterNumber: 212222040019
*/
```

## SOURCE CODE:
```
import java.util.*;
abstract class gamestore{
    abstract int finalscore();
}
class arcade extends gamestore{
    int base,level;
    arcade(int base,int level){
        this.base=base;
        this.level=level;
    }
    int finalscore(){
        return base+(level*100);
    }
}
class puzzle extends gamestore{
    int attempts;
    puzzle(int attempts){
        this.attempts=attempts;
    }
    int finalscore(){
        return (attempts<=3)?1000-(attempts*100):500;
    }
}
public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int choice=sc.nextInt();
        gamestore gg;
        if(choice==1){
            int base=sc.nextInt();
            int level=sc.nextInt();
            gg=new arcade(base,level);
            System.out.println(gg.finalscore());
        }
        else{
            int attempts=sc.nextInt();
            gg=new puzzle(attempts);
            System.out.println(gg.finalscore());
        }
    }
}

```
## OUTPUT:
<img width="325" height="211" alt="image" src="https://github.com/user-attachments/assets/c27cadb9-e7f0-4336-b52f-932a954c9d51" />



## RESULT:
The program was implemented successfully and verified.



