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
#include <iostream>
#include <string>
using namespace std;

class Student
{
private:
    string name;
    string studentClass;
    int roll;
    double marks;

public:
    Student(string n, string c, int r, double m)
    {
        name = n;
        studentClass = c;
        roll = r;
        marks = m;
    }

    string calculateGrade()
    {
        if (marks >= 80)
            return "A+";
        else if (marks >= 70)
            return "A";
        else if (marks >= 60)
            return "A-";
        else if (marks >= 50)
            return "B";
        else if (marks >= 40)
            return "C";
        else
            return "F";
    }

    void display()
    {
        cout << "\nStudent Information:" << endl;
        cout << "Name: " << name << endl;
        cout << "Class: " << studentClass << endl;
        cout << "Roll Number: " << roll << endl;
        cout << "Marks: " << marks << endl;
        cout << "Grade: " << calculateGrade() << endl;
    }
};

int main()
{
    string name, cls;
    int roll;
    double marks;

    cout << "Enter student name: ";
    getline(cin, name);
    cout << "Enter class: ";
    getline(cin, cls);
    cout << "Enter roll number: ";
    cin >> roll;
    cout << "Enter marks: ";
    cin >> marks;

    Student s(name, cls, roll, marks);
    s.display();

    return 0;
}
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
