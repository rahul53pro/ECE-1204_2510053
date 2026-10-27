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
#include<iostream>
using namespace std;
class rectangle
{
private:
    int length;
    int width;
public:
    rectangle(int l, int w)
    {
        length = l;
        width = w;
    }
    float area()
    {
        return length*width;
    }
    float perimeter()
    {
        return 2*(length + width);
    }
};

int main()
{
    rectangle a(2,3);
    cout << "Area : " << a.area() << endl;
    cout << "Perimeter : " << a.perimeter() << endl;
}

```

### Output
<img src="" alt="image-1">

### Discussion

---

## Problem-02

Define a class named “student”. Declare one variable and function for private, public and protected. Define the functions outside of the class. Now try to access the variable and functions from main function and see what happens.

**Status:** Pending

### Code
```cpp
#include <iostream>
#include <string>

using namespace std;

class Student
{
private:
    string name;
    void Name();

protected:
    int roll;
    void Roll();

public:
    string department;
    void Department();
};

void Student::Name()
{
    cout << "NAME: " << name << endl;
}

void Student::Roll()
{
    cout << "ROLL: " << roll << endl;
}

void Student::Department()
{
    cout << "DEPARTMENT: " << department << endl;
}

int main()
{
    Student S;

    // S.name = "Cobra";
    // S.roll = 2510053;
    S.department = "ECE";

    // S.Name();
    // S.Roll();
    S.Department();

    return 0;
}

```

### Sample Output


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
