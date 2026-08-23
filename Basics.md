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
# 📄04:Data Types-
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
📝 Important Points

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

🎯 Summary
```cpp
int       → 10
float     → 10.5f
double    → 10.5555
char      → 'A'
bool      → true / false
void      → no value
```
