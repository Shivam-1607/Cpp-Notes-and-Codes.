# 📄Basics: Header files, Variable, Comments.

## 📄 01:Hello World.cpp

```cpp
#include <iostream>      // Provides input/output functionality
using namespace std;     // Allows us to use cout without writing std::cout 

int main()               // Program execution starts from main()
{
    cout << "Hello, World!";   // Displays text on the screen
    return 0;             // Indicates that the program ended successfully
}
``` 

 ### 📌 Theory

A basic C++ program consists of:

-Header files → Provide predefined functionality.

-Namespace → Organizes identifiers such as cout and cin.

-main() function → Starting point of program execution.

-Statements → Instructions executed by the program.

-return statement → Returns a value from a function.

### 🔹 Basic structure
```cp
#include <header_file>
using namespace namespace_name;
int main()
{
    // Statements
    return 0;
}
```

### 📝 Important points

-C++ is case-sensitive.

-Every normal statement ends with ;.

-main() is the entry point of a C++ program.

-cout is used to display output.

-#include <iostream> provides cout and cin.

-return 0 indicates successful execution.


## 📄 02:Comments.cpp

### 📌 Theory

-Comments are notes written inside source code for humans. They are ignored by the compiler and do not affect program execution.

-C++ supports two types of comments:

Single-line comments → //

*Multi-line comments → /* ... */

### 🔹 Syntax

Single-line:
```cp
// This is a comment
```
Multi-line:
```cp
/*
   This is a
   multi-line comment
*/
```
### 💻 Example
```cp
#include <iostream>
using namespace std;
int main()
{
    // This is a single-line comment
    cout << "Hello";
       /*
       This is a multi-line comment.
       The compiler ignores everything
       written between these symbols.
       */
 cout << " C++";
 return 0;
}
```

### 📝 Important points

_Comments are used to explain code and improve readability.

-Comments are not executed.

-// comments continue until the end of the line.

-/* */ comments can span multiple lines.


## 📄 03:Variables.cpp

### 📌 Theory

-A variable is a named memory location used to store data.

-Every variable has:

>Data Type + Variable Name + Value

*For example:
```cp
int age = 18;
```

=>Here:

-int → data type

-age → variable name

-18 → value

### 🔹 Syntax
```
data_type variable_name = value;
or
data_type variable_name;
variable_name = value;
```
### 💻 Example
```cp
#include <iostream>
using namespace std;
int main()
{
    int age = 18;          // Integer variable
    float marks = 89.5;    // Floating-point variable
    char grade = 'A';      // Character variable
    bool passed = true;    // Boolean variable
     cout << age << endl;
    cout << marks << endl;
    cout << grade << endl;
    cout << passed << endl;
   return 0;
}
```
### 📝 Important points

-A variable must have a data type.

-Variable names are case-sensitive.

-A variable can be assigned a new value after declaration.

```cp
int age = 18;
age = 19;       // Value changed
```
## 📄04:Data Types-
### 📌 Theory

-A data type specifies what kind of data a variable can store and how much memory is generally required to store it.

-C++ has several built-in data types.

🔹 Common C++ Data Types

| Data Type | Used for | Example |
|---|---|---|
| `int` | Whole numbers | `10` |
| `float` | Decimal numbers | `10.5f` |
| `double` | More precise decimal numbers | `10.5678` |
| `char` | Single character | `'A'` |
| `bool` | True/false values | `true` |
| `void` | No value | `void function()` |

🔹 **Syntax**

```cpp
data_type variable_name = value;
```
🔹Example:
```cpp
int age = 19;
💻 Example
#include <iostream>
using namespace std;

int main()
{
    int age = 19;              // Stores whole numbers
    float height = 5.8f;       // Stores decimal numbers
    double price = 99.9999;    // Stores decimal numbers with higher precision
    char grade = 'A';          // Stores a single character
    bool passed = true;        // Stores true or false

    cout << "Age: " << age << endl;
    cout << "Height: " << height << endl;
    cout << "Price: " << price << endl;
    cout << "Grade: " << grade << endl;
    cout << "Passed: " << passed << endl;

    return 0;
}
```
```cpp
Output
Age: 19
Height: 5.8
Price: 99.9999
Grade: A
Passed: 1
```
*By default, C++ prints:

-true  → 1
-false → 0

🔹 Character Data Type

-char stores one character.

-char letter = 'A';

-Characters are written using single quotes.

-char a = 'A';      // Correct

-char a = "A";      // Not correct for a single char

🔹 Boolean Data Type

-bool stores only two possible values:

-true

-false

🔹Example:

```cpp
bool isStudent = true;
bool isWorking = false;
```
🔹 sizeof() Operator

-The sizeof() operator is used to determine the amount of memory occupied by a data type or variable.

```cpp
Syntax
sizeof(variable);
Example
#include <iostream>
using namespace std;

int main()
{
    int a = 10;
    float b = 10.5f;
    double c = 20.55;
    char d = 'A';
    bool e = true;

    cout << "Size of int: " << sizeof(a) << " bytes" << endl;
    cout << "Size of float: " << sizeof(b) << " bytes" << endl;
    cout << "Size of double: " << sizeof(c) << " bytes" << endl;
    cout << "Size of char: " << sizeof(d) << " bytes" << endl;
    cout << "Size of bool: " << sizeof(e) << " bytes" << endl;

    return 0;
}
```
-The exact size of some types can depend on the compiler and platform, although common modern systems typically use:

```cpp
int       → 4 bytes
float     → 4 bytes
double    → 8 bytes
char      → 1 byte
bool      → 1 byte
```
### 📝 Important Points

-int → whole numbers.

-float → decimal numbers with single precision.

-double → decimal numbers with higher precision than float.

-char → one character.

-bool → true or false.

-sizeof() → determines the memory size of a type or variable.

-char values use single quotes.

-C++ is strongly typed, so every variable has a specific type


🔹 Basic Classification

### C++ Data Types

```text
C++ Data Types
│
├── Fundamental
│   ├── int
│   ├── float
│   ├── double
│   ├── char
│   ├── bool
│   └── void
│
├── Derived
│   ├── Array
│   ├── Pointer
│   ├── Reference
│   └── Function
│
└── User-defined
    ├── class
    ├── struct
    ├── union
    └── enum
   ```

### 🎯 Summary
```cpp
int       → 10
float     → 10.5f
double    → 10.5555
char      → 'A'
bool      → true / false
void      → no value
```
 
## 📄05: Constants-

### 📌 Theory

-A constant is a value that cannot be changed after it has been defined.

-In C++, the const keyword is used to make a variable constant.

-Once a value is assigned to a const variable, trying to change it will produce a compilation error.

🔹 Syntax
```cpp
const data_type variable_name = value;
```
*Example:
```cpp
const int MAX_SCORE = 100;
```
### 💻 Example
```cpp
#include <iostream>
using namespace std;

int main()
{
    const int MAX_MARKS = 100;   // Constant value

    cout << "Maximum marks: " << MAX_MARKS << endl;

    // MAX_MARKS = 200;
    // Error: cannot modify a const variable

    return 0;
}
Output
Maximum marks: 100
```
🔹 Constants with Different Data Types
```cpp
#include <iostream>
using namespace std;

int main()
{
    const int age = 19;            // Constant integer
    const float pi = 3.14f;        // Constant float
    const char grade = 'A';        // Constant character
    const double gravity = 9.81;   // Constant double

    cout << age << endl;
    cout << pi << endl;
    cout << grade << endl;
    cout << gravity << endl;

    return 0;
}
```
🔹 Normal Variable vs Constant
```text
-Normal variable
int age = 19;

age = 20;    // Allowed
-Constant variable
const int age = 19;

age = 20;    // Error
```
-The difference is:

-Normal variable → value can be changed

-Constant        → value cannot be changed

🔹 Constants for Fixed Values

-Constants are useful when a value should remain fixed throughout a program.
```cpp
#include <iostream>
using namespace std;

int main()
{
    const double PI = 3.14159;
    double radius = 5;

    double area = PI * radius * radius;

    cout << "Area: " << area << endl;

    return 0;
}
```

-Here, PI should not be changed because its value is fixed.

### 📝 Important Points

-Use const to create a constant variable.

-A constant must normally be initialized when declared.

-Its value cannot be modified after initialization.

-Constants improve code safety and readability.

-Constant names are often written in uppercase by convention.

🔹 Example
```cpp
const int MAX_USERS = 100;
const double PI = 3.14159;
const int DAYS_IN_WEEK = 7;
```
### 🎯 Summary

const
  ↓
Makes a variable read-only
  ↓
Value cannot be changed

-Basic syntax:
```cpp
const data_type variable_name = value;
```
## 📄07: Operators in C++:-

### 📌 Theory

-Operators are symbols used to perform operations on values and variables.

-For example:
```
a + b
```

-Here, + is an operator that performs addition.

-C++ provides several types of operators.

🔹 Types of Operators-

Operators
│
├── Arithmetic Operators
├── Assignment Operators
├── Relational Operators
├── Logical Operators
├── Increment / Decrement Operators
├── Bitwise Operators
└── Conditional Operator

### 1.➕ Arithmetic Operators:-

-Arithmetic operators are used to perform mathematical operations.

| Operator | Operation       | Example |
|----------|-----------------|---------|
| `+`      | Addition        | `a + b` |
| `-`      | Subtraction     | `a - b` |
| `*`      | Multiplication  | `a * b` |
| `/`      | Division        | `a / b` |
| `%`      | Modulus         | `a % b` |

### 💻 Example-`
```cpp

#include <iostream>
using namespace std;

int main()
{
    int a = 10;
    int b = 3;

    cout << "Addition: " << a + b << endl;
    cout << "Subtraction: " << a - b << endl;
    cout << "Multiplication: " << a * b << endl;
    cout << "Division: " << a / b << endl;
    cout << "Remainder: " << a % b << endl;

    return 0;
}
```
-Output:
 ```
Addition: 13
Subtraction: 7
Multiplication: 30
Division: 3
Remainder: 1
```

### ⚠️ Integer Division

-When both operands are integers, / performs integer division.
```
int a = 5;
int b = 2;

cout << a / b;
```
-Output:
```
2
```
-The decimal part is discarded.

### 2.📝 Assignment Operators-

-Assignment operators are used to assign or update values.

| Operator | Example   | Equivalent to |
|----------|-----------|---------------|
| `=`      | `a = 5`   | `a = 5`       |
| `+=`     | `a += 5`  | `a = a + 5`   |
| `-=`     | `a -= 5`  | `a = a - 5`   |
| `*=`     | `a *= 5`  | `a = a * 5`   |
| `/=`     | `a /= 5`  | `a = a / 5`   |
| `%=`     | `a %= 5`  | `a = a % 5`   |

### 💻 Example-
```
#include <iostream>
using namespace std;

int main()
{
    int a = 10;

    a += 5;    // a = a + 5
    cout << a << endl;

    a -= 3;    // a = a - 3
    cout << a << endl;

    a *= 2;    // a = a * 2
    cout << a << endl;

    a /= 4;    // a = a / 4
    cout << a << endl;

    return 0;
}
```

### 3.⚖️ Relational Operators-

-Relational operators compare two values.

-The result is a Boolean value:
```
true  → 1
false → 0
```

| Operator | Meaning                     |
|----------|-----------------------------|
| `==`     | Equal to                    |
| `!=`     | Not equal to                |
| `>`      | Greater than                |
| `<`      | Less than                   |
| `>=`     | Greater than or equal to    |
| `<=`     | Less than or equal to       |

### 💻 Example-
```cpp
#include <iostream>
using namespace std;

int main()
{
    int a = 10;
    int b = 20;

    cout << (a == b) << endl;   // Checks whether a equals b
    cout << (a != b) << endl;   // Checks whether a is not equal to b
    cout << (a < b) << endl;    // Checks whether a is less than b
    cout << (a > b) << endl;    // Checks whether a is greater than b
    cout << (a <= b) << endl;   // Checks whether a is less than or equal to b
    cout << (a >= b) << endl;   // Checks whether a is greater than or equal to b

    return 0;
}
````

### 4. 🧠 Logical Operators-

-Logical operators are used to combine or modify conditions.

| Operator | Name         | Meaning                         |
|----------|--------------|---------------------------------|
| `&&`     | Logical AND  | Both conditions must be true    |
| `||`     | Logical OR   | At least one condition is true  |
| `!`      | Logical NOT  | Reverses the result             |

### 💻 Example-
```cpp
#include <iostream>
using namespace std;

int main()
{
    int age = 20;
    bool hasID = true;

    // Both conditions must be true
    cout << (age >= 18 && hasID) << endl;

    // At least one condition must be true
    cout << (age >= 18 || hasID) << endl;

    // Reverses true to false or false to true
    cout << !hasID << endl;

    return 0;
}
```

### 5. 🔼 Increment and Decrement Operators-

-These operators increase or decrease a variable by 1.

| Operator | Operation       |
|----------|-----------------|
| `++`     | Increment by 1  |
| `--`     | Decrement by 1  |

### 💻 Example-
```cpp
#include <iostream>
using namespace std;

int main()
{
    int a = 5;

    a++;    // Increases a by 1
    cout << a << endl;    // 6

    a--;    // Decreases a by 1
    cout << a << endl;    // 5

    return 0;
}
```
🔹 Prefix and Postfix

-Increment and decrement operators can be used before or after a variable.
```
Prefix
++a;
```
-The value is changed before it is used in the expression.
```
Postfix
a++;
```
-The original value is used first, then the variable is incremented.

*Example-
```cpp
#include <iostream>
using namespace std;

int main()
{
    int a = 5;

    cout << ++a << endl;   // Increment first, then print → 6

    a = 5;

    cout << a++ << endl;   // Print first, then increment → 5
    cout << a << endl;     // a is now 6

    return 0;
}
```
### 6. 💻 Bitwise Operators-

-Bitwise operators work directly with the individual bits of integer values.

| Operator | Name          |
|----------|---------------|
| `&`      | Bitwise AND   |
| `|`      | Bitwise OR    |
| `^`      | Bitwise XOR   |
| `~`      | Bitwise NOT   |
| `<<`     | Left Shift    |
| `>>`     | Right Shift   |

### 💻 Example-
```cpp
#include <iostream>
using namespace std;

int main()
{
    int a = 5;    // Binary: 0101
    int b = 3;    // Binary: 0011

    cout << (a & b) << endl;   // Bitwise AND
    cout << (a | b) << endl;   // Bitwise OR
    cout << (a ^ b) << endl;   // Bitwise XOR

    return 0;
}
```

-Bitwise operators become particularly important when studying low-level programming, systems, embedded programming, and computer architecture.

### 7.❓ Conditional / Ternary Operator-

-The conditional operator is a short way of writing a simple if-else expression.

🔹 Syntax
```
condition ? expression1 : expression2;
```
-If the condition is true, expression1 is selected. Otherwise, expression2 is selected.

### 💻 Example:
```cpp
#include <iostream>
using namespace std;

int main()
{
    int age = 20;

    // If age >= 18, result becomes "Adult"
    // Otherwise, result becomes "Minor"
    string result = (age >= 18) ? "Adult" : "Minor";

    cout << result;

    return 0;
}
```
-Output:
```
Adult
```
### 📝 Operator Precedence-

-When an expression contains multiple operators, C++ follows operator precedence to determine the order of evaluation.

-For example:
```
int result = 2 + 3 * 4;
```
-Multiplication is performed before addition:
```
3 * 4 = 12
2 + 12 = 14
```
-Therefore:
```
result = 14
```
-Parentheses can be used to explicitly control the order:
```
int result = (2 + 3) * 4;
```
-Now:
```
2 + 3 = 5
5 * 4 = 20
```
### 🎯 Summary-

| Operators              | Category                  |
|------------------------|---------------------------|
| `+ - * / %`            | Arithmetic                |
| `= += -= *= /= %=`     | Assignment                |
| `== != > < >= <=`      | Relational                |
| `&& || !`              | Logical                   |
| `++ --`                | Increment / Decrement     |
| `& | ^ ~ << >>`        | Bitwise                   |
| `? :`                  | Conditional (Ternary)     |
