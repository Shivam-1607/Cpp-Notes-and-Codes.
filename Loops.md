# 📄14.for Loop-

## 📌 Theory

-A `for` loop is used to **repeat a block of code** a specific number of times.

-It has three main parts:

1. **Initialization** — starts the loop variable.
 
2. **Condition** — decides whether the loop continues.
 
3. **Update** — changes the loop variable after each iteration.

## 🔹 Syntax-

```cpp
for (initialization; condition; update)
{
    // Statements to repeat
}
```

## 💻 Example-

```cpp
#include <iostream>
using namespace std;

int main()
{
    // Start i at 1, continue while i <= 5,
    // and increase i by 1 after every iteration
    for (int i = 1; i <= 5; i++)
    {
        cout << i << endl;
    }

    return 0;
}
```

### Output-

```text
1
2
3
4
5
```

## 🔹 How It Works-

-For this loop:

```cpp
for (int i = 1; i <= 5; i++)
```

-The execution is:

```text
Initialization → int i = 1
       ↓
Check condition → i <= 5
       ↓
Execute loop body
       ↓
Update → i++
       ↓
Check condition again
       ↓
Repeat
```

-When `i` becomes `6`, the condition `i <= 5` becomes false and the loop stops.

## 🔹 Printing Even Numbers-

```cpp
#include <iostream>
using namespace std;

int main()
{
    // Start from 2 and increase by 2
    // This prints only even numbers
    for (int i = 2; i <= 10; i += 2)
    {
        cout << i << " ";
    }

    return 0;
}
```

### Output-

```text
2 4 6 8 10
```

## 🔹 Reverse Loop-

-A `for` loop can also run backwards.

```cpp
#include <iostream>
using namespace std;

int main()
{
    // Start at 5 and decrease i by 1
    for (int i = 5; i >= 1; i--)
    {
        cout << i << " ";
    }

    return 0;
}
```

### Output-

```text
5 4 3 2 1
```

## 📝 Important Points-

* `for` loops are useful when the number of repetitions is known or controlled by a counter.
  
* Initialization runs only once
  
* The condition is checked before each iteration.
  
* The update runs after the loop body.
  
* `i++` increases `i` by 1.
  
* `i--` decreases `i` by 1.
  
* A loop can execute zero times if its condition is false initially.

## 🎯 Summary-

```text
for loop
   │
   ├── Initialization
   │
   ├── Condition
   │      │
   │    True
   │      ↓
   │   Loop Body
   │      ↓
   │    Update
   │      │
   │      └────→ Condition
   │
   └── False → Stop
```
