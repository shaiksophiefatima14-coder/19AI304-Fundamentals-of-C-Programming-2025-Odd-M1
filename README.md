# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 07-08-25
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
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
    int intLiteral = 10;
    float floatLiteral = 3.14;
    char charLiteral = 'A';
    char strLiteral[] = "Hello C";

    printf("Integer literal: %d\n", intLiteral);
    printf("Size of intLiteral: %zu bytes\n\n", sizeof(intLiteral));

    printf("Float literal: %.2f\n", floatLiteral);
    printf("Size of floatLiteral: %zu bytes\n\n", sizeof(floatLiteral));

    printf("Character literal: %c\n", charLiteral);
    printf("Size of charLiteral: %zu bytes\n\n", sizeof(charLiteral));

    printf("String literal: %s\n", strLiteral);
    printf("Size of strLiteral: %zu bytes\n", sizeof(strLiteral));

    return 0;
}

```
# Output:
<img width="414" height="322" alt="image" src="https://github.com/user-attachments/assets/bd88d83a-7d65-481b-b075-6d435d35c084" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 07-08-25
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
#define PI 3.14159

int main() {
    const int DAYS = 7;

    printf("Value of macro constant PI: %.5f\n", PI);
    printf("Value of constant variable DAYS: %d\n", DAYS);

    return 0;
}
```

# Output:
<img width="397" height="100" alt="image" src="https://github.com/user-attachments/assets/b0c18407-beb1-462e-8e9e-f04f22a775d3" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 09-08-25
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
    int intVar = 25;
    float floatVar = 3.14f;
    double doubleVar = 3.1415926535;
    char charVar = 'Z';

    printf("Integer value: %d\n", intVar);
    printf("Float value: %.2f\n", floatVar);
    printf("Double value: %.10lf\n", doubleVar);
    printf("Character value: %c\n", charVar);

    return 0;
}
```
# Output:
<img width="298" height="135" alt="image" src="https://github.com/user-attachments/assets/bb60b53c-80e6-4d03-8727-4a34f5831f54" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 09-08-25
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

    // Input values for a and b
    printf("Enter two integers (a and b): ");
    scanf("%d %d", &a, &b);

    // Arithmetic operations
    printf("\nArithmetic Operations:\n");
    printf("Sum (a + b) = %d\n", a + b);
    printf("Difference (a - b) = %d\n", a - b);
    printf("Product (a * b) = %d\n", a * b);

    if (b != 0) {
        printf("Quotient (a / b) = %d\n", a / b);
        printf("Remainder (a %% b) = %d\n", a % b);
    } else {
        printf("Quotient and Remainder: Division by zero error!\n");
    }

    // Bitwise operations
    printf("\nBitwise Operations:\n");
    printf("AND (a & b) = %d\n", a & b);
    printf("OR (a | b) = %d\n", a | b);
    printf("XOR (a ^ b) = %d\n", a ^ b);
    printf("Left shift (a << b) = %d\n", a << b);
    printf("Right shift (a >> b) = %d\n", a >> b);
    printf("Bitwise NOT of a (~a) = %d\n", ~a);
    printf("Bitwise NOT of b (~b) = %d\n", ~b);

    return 0;
}
```
# Output:
<img width="413" height="477" alt="image" src="https://github.com/user-attachments/assets/9ba4b7b1-dd72-4bb6-97c4-8b8166b8a642" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 09-08-25
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
    printf("Enter a character: ");
    scanf("%c", &ch);
    if (ch >= '0' && ch <= '9'){
        printf("Digit\n");
    }
    else {
        if ((ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z')) {
            if (ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U' ||
                ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u') {
                printf("Vowel\n");
            } else {
                printf("Consonant\n");
            }
        }
        else {
            printf("Special Symbol\n");
        }
    }
    return 0;
}
```
# Output:
<img width="332" height="84" alt="image" src="https://github.com/user-attachments/assets/2850a478-d170-48be-be14-cfae06bedf11" />

<img width="288" height="100" alt="image" src="https://github.com/user-attachments/assets/8cd706a0-c033-48a5-b8dc-cc4c5100b508" />

<img width="249" height="86" alt="image" src="https://github.com/user-attachments/assets/c0ed647e-a316-45cb-b0d4-69f303521c91" />

<img width="261" height="74" alt="image" src="https://github.com/user-attachments/assets/2a6ad49a-2a23-4833-b19e-3c24b91dff2b" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


