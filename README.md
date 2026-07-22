# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 18-07-2026.
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard iput-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
```
#include <stdio.h>
int main() {
    int my_int = 100;
    float my_float = 5.75f;
    char my_char = 'Z';
    char my_string[] = "Welcome";
    printf("Integer literal: %d\n", my_int);
    printf("Float literal: %.2f\n", my_float);
    printf("Character literal: %c\n", my_char);
    printf("String literal: %s\n", my_string);
}
```
# Output:
<img width="256" height="105" alt="image" src="https://github.com/user-attachments/assets/d1392991-f407-419f-be9a-ae374bfac0f7" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 18-07-2026.
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
```
#include <stdio.h>
#define MAX 50
int main() {
    const int MIN = 10;
    printf("Macro: %d\n", MAX);
    printf("Constant: %d\n", MIN);
}
```
# Output:

<img width="189" height="53" alt="image" src="https://github.com/user-attachments/assets/0cbe4441-fb95-472e-8af8-0c3501f5a66c" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 18-07-2026.
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
```
#include <stdio.h>
int main() {
    int age = 20;
    float height = 5.9f;
    double pi = 3.1415926535;
    char grade = 'A';
    printf("Integer value: %d\n", age);
    printf("Float value: %.1f\n", height);
    printf("Double value: %.10lf\n", pi);
    printf("Character value: %c\n", grade);
    return 0;
}
```
# Output:
<img width="264" height="101" alt="image" src="https://github.com/user-attachments/assets/1898f5c6-b8cc-49c6-ae00-b9c9aa06925e" />

# Result: 

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 18-07-2026.
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>
int main() {
    int a, b;
    scanf("%d %d", &a, &b);
    printf("Addition (a + b)        = %d\n", a + b);
    printf("Subtraction (a - b)     = %d\n", a - b);
    printf("Multiplication (a * b)  = %d\n", a * b);
    if (b != 0) {
        printf("Division (a / b)        = %d\n", a / b);
        printf("Remainder (a %% b)       = %d\n", a % b);
    } else {
        printf("Division & Remainder   = Cannot divide by zero\n");
    }
    printf("Bitwise AND (a & b)     = %d\n", a & b);
    printf("Bitwise OR (a | b)      = %d\n", a | b);
    printf("Bitwise XOR (a ^ b)     = %d\n", a ^ b);
    printf("Left Shift (a << 1)     = %d\n", a << 1);
    printf("Right Shift (a >> 1)    = %d\n", a >> 1);
    printf("Bitwise NOT (~a)        = %d\n", ~a);
    return 0;
}
```
# Output:
<img width="327" height="299" alt="image" src="https://github.com/user-attachments/assets/44d20572-d162-4e43-88fb-a7b19e055734" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 18-07-2026.
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>
int main() {
    char ch;
    scanf("%c", &ch);
    (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' ||
     ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U') 
     ? printf("'%c' is a Vowel.\n", ch)
     : ((ch >= 'a' && ch <= 'z') || (ch >= 'A' && ch <= 'Z'))
        ? printf("'%c' is a Consonant.\n", ch)
        : (ch >= '0' && ch <= '9')
            ? printf("'%c' is a Digit.\n", ch)
            : printf("'%c' is a Special Symbol.\n", ch);
    return 0;
}
```
# Output:
<img width="170" height="56" alt="image" src="https://github.com/user-attachments/assets/cbed93e3-9ffd-48b4-ab44-2262f8fe0854" />
<img width="153" height="41" alt="image" src="https://github.com/user-attachments/assets/7b3a0a06-6825-41ed-9d0f-1f0ae34950fd" />
<img width="231" height="52" alt="image" src="https://github.com/user-attachments/assets/a9996b61-4b71-4b07-9fe8-fa6b76d9ee0a" />
<img width="196" height="56" alt="image" src="https://github.com/user-attachments/assets/00b5543f-0661-4f0b-a11c-5a08af4b712c" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


