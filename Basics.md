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
