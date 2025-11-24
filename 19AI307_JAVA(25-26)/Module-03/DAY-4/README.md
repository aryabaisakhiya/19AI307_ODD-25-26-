# Ex.No:3(D)    INTERFACE 

## QUESTION:
You're building the equalizer system for a music app like BeatBoxx. The equalizer has 3 basic sound modes:

BassBoost
VocalBoost
Balanced
Each mode behaves differently and alters the sound experience. The app uses a SoundMode interface that each mode implements.


## AIM:
To create a sound equalizer system using an interface SoundMode that is implemented by three classes—BassBoost, VocalBoost, and Balanced—each providing its own sound-enhancing behavior.

## ALGORITHM :
```
1.Start
2.Create an interface SoundMode with a method like applyMode()
3.Implement three classes BassBoost, VocalBoost, and Balanced, each giving its own version of the sound effect
4.Create objects of each mode and call applyMode() to display how the sound is modified
5.Output the behavior of each mode and end
```

## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: Arya Baisakhiya
RegisterNumber: 212222040019
*/
```

## SOURCE CODE:
```
import java.util.*;

interface SoundMode {
    void applySettings();
}

class BassBoost implements SoundMode {
    public void applySettings() {
        System.out.println("Bass Boost applied. Feel the beat drop!");
    }
}

class VocalBoost implements SoundMode {
    public void applySettings() {
        System.out.println("Vocal Boost enabled. Enjoy crystal-clear lyrics!");
    }
}

class Balanced implements SoundMode {
    public void applySettings() {
        System.out.println("Balanced mode set. A perfect blend of bass and vocals.");
    }
}

public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String mode = sc.next().toLowerCase();
        
        SoundMode soundMode;
        
        switch (mode) {
            case "bass":
                soundMode = new BassBoost();
                break;
            case "vocal":
                soundMode = new VocalBoost();
                break;
            case "balanced":
                soundMode = new Balanced();
                break;
            default:
                System.out.println("Invalid mode selected.");
                return;
        }
        
        soundMode.applySettings();
    }
}
```
## OUTPUT:
<img width="1078" height="226" alt="image" src="https://github.com/user-attachments/assets/a0d1f4aa-bc8d-4f45-ab14-4293beac4c7d" />



## RESULT:
The program was implemented successfully and verified.



