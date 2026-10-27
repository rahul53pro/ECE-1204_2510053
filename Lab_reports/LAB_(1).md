# Lab 01: OOP Classes and Objects

| | |
| :--- | :--- |
| **Course** | ECE 1204 – Object Oriented Programming Sessional |
| **Lab Workout** | Defining a class with private data members and member functions |
| **Submission Date** | 28 Oct 2026 |

---

## Table of Contents
1. [Problem-01](#problem-01)
2. [Problem-02](#problem-02)
3. [Problem-03](#problem-03)
4. [Problem-04](#problem-04)

---

## Problem-01

**Problem Statement:** Write a C++ program to create a class called `Rectangle` that has private member variables for length and width. Implement member functions to calculate the rectangle's area and perimeter.

**Status:** Done

### Code
```cpp
#include <iostream>

using namespace std;

class Rectangle {
private:
    float length;
    float width;

public:
    Rectangle(float l, float w) {
        length = l;
        width = w;
    }

    float area() {
        return length * width;
    }

    float perimeter() {
        return 2 * (length + width);
    }
};

int main() {
    Rectangle rect(5, 3);

    cout << "Area: " << rect.area() << endl;
    cout << "Perimeter: " << rect.perimeter() << endl;

    return 0;
}
```

### Sample Output
```text
Enter length: 5
Enter width: 3
Area = 15
Perimeter = 16
```

### Discussion
The `length` and `width` variables are declared `private`, so they cannot be accessed directly from `main()`. They are set through the constructor, and the public member functions `area()` and `perimeter()` use them to return the results. This is **encapsulation**: the data is protected inside the class and used only through its own functions. Both functions are marked `const` because they only read the data and do not change the object.

---

## Problem-02

**Problem Statement:** _Write the problem statement here._

**Status:** Pending

### Code
```cpp
#include <iostream>
using namespace std;

int main() {
    // Write your C++ code here

    return 0;
}
```

### Sample Output
```text
Paste the program output here
```

### Discussion
_Write a short explanation of your approach and what you learned._

---

## Problem-03

**Problem Statement:** _Write the problem statement here._

**Status:** Pending

### Code
```cpp
#include <iostream>
using namespace std;

int main() {
    // Write your C++ code here

    return 0;
}
```

### Sample Output
```text
Paste the program output here
```

### Discussion
_Write a short explanation of your approach and what you learned._
