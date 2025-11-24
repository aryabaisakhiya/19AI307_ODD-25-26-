# Ex.No:5(A) INPUTSTREAMREADER 

## QUESTION:
Write a Java program to write characters to a file using FileWriter.

## AIM:
To write a Java program that writes character data into a text file using the FileWriter class.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a FileWriter object and specify the filename.
4. Write characters to the file using the write() method.
5. Close the FileWriter to save the data.
6. End the program.

## PROGRAM:
 ```
Program to implement a InputStreamReader using Java
Developed by: Arya Baisakhiya
Register Number: 212222040019
```

## SOURCE CODE:
```
import java.io.*;
import java.util.Scanner;
public class FileWriterExampleUserInput {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        try {
            String fileName = sc.nextLine();
            String content = sc.nextLine();
            FileWriter fw = new FileWriter(fileName);
            fw.write(content);
            fw.close();
            System.out.println("File written successfully.");
        }
        catch (IOException e) {
            System.out.println("Error writing to file: " + e.getMessage());
        }
        finally {
            sc.close();
        }
    }
}
```

## OUTPUT:
<img width="762" height="311" alt="image" src="https://github.com/user-attachments/assets/ecd16df4-219c-433b-9992-995f741b0f0d" />


## RESULT:
The program was implemented successfully and verified.




