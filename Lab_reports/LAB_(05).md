# Lab 03: 

| | |
| :--- | :--- |
| **Course** | ECE 1204 – Object Oriented Programming Sessional |
| **Lab Workout** | |
| **Submission Date** | |

---

## Table of Contents
1. [Problem-01](#problem-01)
2. [Problem-02](#problem-02)
3. [Problem-03](#problem-03)


---

## Problem-01
**Problem Statement:** 

**Status:** Done

### Code
```cpp
#include <iostream>
#include <cmath>
using namespace std;

class Shape
{
public:
    virtual float area()
    {
        return 0;
    }
    virtual float perimeter()
    {
        return 0;
    }
};

class Circle : public Shape
{
    float r;
public:
    Circle(float rad)
    {
        r = rad;
    }
    float area()
    {
        return 3.1416 * r * r;
    }
    float perimeter()
    {
        return 2 * 3.1416 * r;
    }
};

class Rectangle : public Shape
{
    float l, w;
public:
    Rectangle(float len, float wid)
    {
        l = len;
        w = wid;
    }
    float area()
    {
        return l * w;
    }
    float perimeter()
    {
        return 2 * (l + w);
    }
};

int main()
{
    Shape *ptr;

    float r, l, w;

    Circle cir(5);
    ptr = &cir;
    cout << "Circle Area: " << ptr->area() << endl;
    cout << "Circle Perimeter: " << ptr->perimeter() << endl << endl;

    Rectangle rec(5, 4);
    ptr = &rec;
    cout << "Rectangle Area: " << ptr->area() << endl;
    cout << "Rectangle Perimeter: " << ptr->perimeter() << endl << endl;

    return 0;
}
```

### Output

<img src="">

### Discussion


---

## Problem-02
**Problem Statement:** 

**Status:** Done

### Code
```cpp

```

### Output

<img src="">

### Discussion


---

## Problem-03
**Problem Statement:** 

**Status:** Done

### Code
```cpp

```

### Output

<img src="">

### Discussion


---
