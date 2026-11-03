# Lab 02: 

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
4. [Problem-04](#problem-04)
5. [Problem-05](#problem-05)

---

## Problem-01
Define a class named “student”. Declare one variable and function for private, public and protected. Define the functions outside of the class. Now try to access the variable and functions from main function and see what happens.
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

### Output

<img src="https://github.com/rahul53pro/ECE-1204_2510053/blob/main/Outputs/LAB-1/Screenshot%202026-10-28%20035123.png" alt="image-1">

### Discussion

---

## Problem-02

**Problem Statement:** Implement a program that demonstrates both friend class and friend function in C++.
1. Class B should be a friend class of class A, and use it to print a private value from A.
2. Also create a friend function that can access and print the same private value of class A.

**Status:** Done

### Code
```cpp
#include<iostream>
using namespace std;
class A
{
private:
    int value;
public:
    A(int v) {
        value = v;
    }
    friend class B;
    friend void printF(A obj);
};
class B {
public:
    void print(A obj) {
        cout << "Using Friend Class B : " << obj.value << endl;
    }
};
void printF(A obj) {
    cout << "Using Friend Function: " << obj.value << endl;
}

int main ()
{
    A object1(2510053);
    B object2;
    object2.print(object1);
    printF(object1);
    
    return 0;
}
```

### Output

<img src="https://github.com/rahul53pro/ECE-1204_2510053/blob/main/Outputs/LAB-2/Screenshot%202026-11-04%20041609.png" alt="image-2">

### Discussion

---

## Problem-03

**Problem Statement:** Design a system for a company that has two types of employees: PermanentEmployee and ContractEmployee. The company also has a HRDepartment that needs access to private data of all employees to calculate bonuses.
Implement the following:
1. A base class Employee that stores basic information: name, employeeID, and baseSalary.
         o Use a constructor to initialize these values.
2. Create two derived classes:
         o PermanentEmployee: Has yearsOfService.
         o ContractEmployee: Has contractDuration.
3. Create a friend class HRDepartment that:
         o Has access to the private data of all employees.
         o Can calculate and display the bonus:
                 $ PermanentEmployee: 10% of base salary + 1000 for each year of service.
                 $ ContractEmployee: 5% of base salary.
Use proper inheritance, constructor chaining, and the friend class concept.

**Status:** Done

### Code
```cpp

```

### Output

<img src="" alt="image-3">

### Discussion

---

## Problem-04
Write a C++ program that calculates the volume of a cube.
**Problem Statement:** 

**Status:** Done

### Code
```cpp
#include <iostream>
using namespace std;
class Cube
{
private:
    float side;
public:
    Cube(float s)
    {
        side = s;
    }
    float volume()
    {
       return side * side * side;
    }
};

int main()
{
    Cube S(5);
    cout << "Volume of cube: " << S.volume() << endl;
    return 0;
}
```

### Output

<img src="" alt="image-4">

### Discussion

---

## Problem-05

**Problem Statement:** 

**Status:** Done

### Code
```cpp

```

### Output

<img src="" alt="image-5">

### Discussion

---
