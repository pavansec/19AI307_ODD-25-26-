# Ex.No:4(A) EXCEPTION HANDLING
### QUESTION:
You wrote a program that stores input strings into a String array and prints each string in uppercase.  
However, you encounter a **NullPointerException**.  

**What should you check in your array before calling `.toUpperCase()` on an element?**

---

### AIM:
To understand how to avoid `NullPointerException` by checking for null values before performing string operations such as `.toUpperCase()`.

---

### ALGORITHM:

1. Read a string input.  
2. Before calling `.toUpperCase()`, check whether the string is `null`.  
3. If it is null, print an appropriate message.  
4. Otherwise, convert the string to uppercase and print it.  
5. End the program safely without exceptions.

---

### PROGRAM:

```
Program to check for null before calling .toUpperCase() on a string
Developed by: PAVAN KUMAR A B
RegisterNumber: 212222040113
```

---

### What should you check?

Before calling:  
```
str.toUpperCase()
```

You **must check**:

```
if (str != null)
```

Otherwise calling `.toUpperCase()` on `null` will throw a `NullPointerException`.

---

### Sourcecode.java:

```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        String input = sc.nextLine();
        
        if (input == null || input.equals("null"))
            System.out.println("Null element");
        else
            System.out.println(input.toUpperCase());
    }
}
```

---

### OUTPUT:
<img width="701" height="243" alt="image" src="https://github.com/user-attachments/assets/621fa0f1-ba5f-455c-a0ad-0256b365ed5b" />


---

### RESULT:
Thus, the program demonstrates that a null check must be done before performing operations like `.toUpperCase()` on a String to avoid `NullPointerException`.

