<img width="829" height="254" alt="image" src="https://github.com/user-attachments/assets/0378a14e-f0a3-46b4-8bfb-d6dc85973c3d" />## Ex.No:1(E) STRINGS AND MATH FUNCTION
### QUESTION:
Write a Java program to read a sentence and determine the longest word present in it.

Example:

Input:  
```
Apple Orange
```
Output:  
```
The longest word is: Orange
```

---

### AIM:
To write a Java program that processes a sentence, splits it into words, and identifies the longest word among them.

---

### ALGORITHM:

1. Read the entire sentence as a string input from the user.  
2. Split the sentence into individual words using whitespace as the delimiter.  
3. Initialize a variable to store the longest word found so far.  
4. Compare the length of each word with the current longest word and update when necessary.  
5. Display the longest word.

---

### PROGRAM:

```
Program to find the longest word in a given sentence
Developed by: PAVAN KUMAR A B
RegisterNumber: 212222040113
```

---

### Sourcecode.java:

```java
import java.util.*;

public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        String sen = sc.nextLine();
        
        String[] words = sen.split("\\s+");
        String longestWord = "";
        
        for(String word : words){
            if(word.length() > longestWord.length()){
                longestWord = word;
            }
        }
        
        System.out.print("The longest word is: " + longestWord); 
        sc.close();
    }
}
```

---

### OUTPUT:
<img width="829" height="254" alt="image" src="https://github.com/user-attachments/assets/93fe4952-69e1-4607-aba8-4766689a0ecc" />


---

### RESULT:
Thus, the Java program to find the longest word in a sentence was successfully executed.

