# 📄1.Type Casting-

###📌 Theory

-Type casting is the process of converting a value from one data type to another.

-For example, converting an int into a float:
```cpp
int a = 10;
float b = (float)a;
```
-C++ supports both implicit and explicit type conversion.

🔹 1. Implicit Type Conversion-

-Implicit conversion happens automatically by the compiler when converting one compatible type to another.

-Example.
```cpp
#include <iostream>
using namespace std;

int main()
{
    int a = 10;
    double b = a;    // int is automatically converted to double

    cout << b;

    return 0;
}
```
-Output:
```
10
```
-Here:

-int → double

-The conversion happens automatically.

🔹 2. Explicit Type Conversion-

-Explicit conversion is performed manually by the programmer.

-Syntax:
```cpp
(type) value;
```
-Example:
```cpp
#include <iostream>
using namespace std;

int main()
{
    double num = 10.75;

    int result = (int)num;    // Explicitly converts double to int

    cout << result;

    return 0;
}
```
-Output:
```
10
```
-The decimal part is removed when converting double to int.

🔹 C++ Cast Syntax-

-C++ also provides a more modern syntax called static_cast.

-Syntax:
```cpp
static_cast<new_type>(value);
```
-Example:
```cpp
#include <iostream>
using namespace std;

int main()
{
    double num = 10.75;

    int result = static_cast<int>(num);  // Converts double to int

    cout << result;

    return 0;
}
```
-Output:
```
10
```
-static_cast is generally preferred over the old C-style (int) syntax because it makes the conversion more explicit.

🔹 Integer to Floating-Point-
```cpp
#include <iostream>
using namespace std;

int main()
{
    int a = 5;

    double b = static_cast<double>(a);

    cout << b;

    return 0;
}
```
-Output:
```
5
```
-The value is now stored as a double.

🔹 Floating-Point to Integer-
```cpp
#include <iostream>
using namespace std;

int main()
{
    double a = 5.99;

    int b = static_cast<int>(a);

    cout << b;

    return 0;
}
```
-Output:
```
5
```
-The fractional part is discarded; this does not round the number.

🔹 Character to Integer-

-Characters have corresponding integer character codes.
```cpp
#include <iostream>
using namespace std;

int main()
{
    char ch = 'A';

    int value = static_cast<int>(ch);  // Converts character to its integer code

    cout << value;

    return 0;
}
```
-For typical ASCII-based systems:
```
'A' → 65
```
🔹 Integer to Character-

-The reverse conversion is also possible.
```cpp
#include <iostream>
using namespace std;

int main()
{
    int value = 65;

    char ch = static_cast<char>(value);  // Converts integer code to character

    cout << ch;

    return 0;
}
```
-Output:
```
A
```
🔹 Type Casting in Division-

-Type casting is particularly useful when performing division.

-Without casting:
```cpp
#include <iostream>
using namespace std;

int main()
{
    int a = 5;
    int b = 2;

    cout << a / b;    // Integer division

    return 0;
}
```
-Output:
```
2
```
-With casting:
```cpp
#include <iostream>
using namespace std;

int main()
{
    int a = 5;
    int b = 2;

    double result = static_cast<double>(a) / b;

    cout << result;

    return 0;
}
```
-Output:
```
2.5
```
-Casting a to double causes the division to be performed using floating-point arithmetic.

### 📝 Important Points:-

-Implicit conversion → performed automatically by the compiler.

-Explicit conversion → performed manually by the programmer.

-static_cast<type>(value) is the standard C++ syntax for many basic conversions.

-Converting double to int discards the fractional part.

-Casting can be useful for obtaining decimal results from integer division.

-Be careful when converting between incompatible types because information can be lost.

### 🎯 Summary:

Type Casting
     │
     ▼
┌─────────────┐
│ Type Casting│
└──────┬──────┘
       │
       ▼
   ┌─────────┐
   │  Types  │
   └────┬────┘
        │
   ┌────┴─────┐
   ▼          ▼
Implicit    Explicit
   │            │
   ▼            ▼
Automatic    Manual
Conversion   Conversion
                │
          ┌─────┴─────┐
          ▼           ▼
     (int)value   static_cast<int>
    
*Common syntax-
```
static_cast<new_type>(value);
```
*Example-
```
double x = 10.5;
int y = static_cast<int>(x);

y becomes 10.
```
