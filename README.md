# CDS-experiment-11

## AIM:-to study and implement classes and objects<br>

### Software used:- VS code<br>

### Theory:-<br>
In C++ (an object-oriented programming language, or OOP), a class is a blueprint that defines the properties (data) and behaviors (methods) of objects. An object is an instance of a class, representing a specific entity that can hold data and interact with other objects using the methods defined in its class.

1).Encapsulation is the process of combining methods (functions) that manipulate data with data (attributes) into a single unit known as a class. This presents simply a controlled interface, concealing the internal state of the objects.<br>
2).Inheritance: A mechanism that encourages code reuse by allowing a new class (derived) to inherit attributes and methods from an existing class (base).<br>
3).Polymrphism:The ability to consider objects of multiple classes as objects of a common base class is known as polymorphism, and it is very helpful for writing reusable and adaptable code.<br>
4).Abstraction: Modeling relevant classes for a given problem while disregarding unimportant features in order to simplify complex reality.<br>


### Code:
```
#include <iostream>
#include <string>

class Student {
private:
    std::string name;
    int rollNumber;
    float marks;
    char grade;

public:
    // Method to set student details
    void setDetails(std::string n, int r, float m) {
        name = n;
        rollNumber = r;
        marks = m;
        calculateGrade();
    }

    // Method to calculate grade based on marks
    void calculateGrade() {
        if (marks >= 90) {
            grade = 'A';
        } else if (marks >= 75 ) {
            grade = 'B';
        } else if (marks >= 60) {
            grade = 'C';
        } else if (marks >= 50) {
            grade = 'D';
        } else {
            grade = 'F';
        }
    }

    // Method to display student details
    void display() {
        std::cout << "Name: " << name << std::endl;
        std::cout << "Roll Number: " << rollNumber << std::endl;
        std::cout << "Marks: " << marks << std::endl;
        std::cout << "Grade: " << grade << std::endl;
    }
};

int main() {
    // Creating a student object and setting details
    Student student1;
    student1.setDetails("Sakalya", 142, 95.6);
    student1.display();

    std::cout << std::endl;

    // Creating another student object and setting details
    Student student2;
    student2.setDetails("Tiya", 144, 92.1);
    student2.display();

    return 0;
}
```
### Output:
![image](https://github.com/user-attachments/assets/01e04128-e9bb-4d4e-b7d9-2d0f3d4a63ca)

### Conclusion:
 1. We learnt how to create classes and objects and how to implement them in C++
 2. We learnt the advantages, disadvatages and application of classes and objects


