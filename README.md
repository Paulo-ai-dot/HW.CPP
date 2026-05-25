# HW.CPP - C++ Object-Oriented Programming Homework

A comprehensive collection of C++ programs demonstrating fundamental Object-Oriented Programming (OOP) concepts and principles. This repository contains practical examples of inheritance, polymorphism, memory management, and advanced class design patterns.

## Repository Contents

### Core Concepts Demonstrated

This homework repository covers essential C++ OOP topics through practical, executable code examples:

#### 1. **Static Members & Class Variables** (`HW6.CPP`)
Demonstrates the use of static member variables that are shared across all instances of a class. The program creates a `Basic` class where a static counter increments with each object instantiation. Each instance maintains its own `class_num` while sharing a common `static_num` counter, illustrating how static members persist across object lifetimes.

#### 2. **Constructor Inheritance & Overloading** (`c.cpp`)
Showcases constructor chaining and parameterized constructors in inheritance hierarchies. The `Derived` class demonstrates calling parent class constructors using initializer lists (`:Base(n1)`), showing how derived classes can invoke and customize base class constructors with different parameters.

#### 3. **Access Modifiers & Encapsulation** (`code.cpp`)
Illustrates the three levels of access control in C++: `private`, `protected`, and `public`. The `Base` class demonstrates how private members are inaccessible even to derived classes, protected members are accessible only to derived classes, and public members are globally accessible. This is fundamental to proper encapsulation.

#### 4. **Constructor & Destructor Order** (`d.cpp`)
Demonstrates the precise order of constructor and destructor invocation in inheritance chains. When objects are created and destroyed, constructors execute from base to derived, while destructors execute in reverse order (derived to base). This is critical for proper resource management.

#### 5. **Multiple Inheritance** (`m.cpp`)
Shows how a single class can inherit from multiple parent classes. The `Final` class inherits from both `Midl` and `Mid2`, demonstrating how to initialize multiple parent classes through the constructor initialization list and access methods from all parent classes.

#### 6. **Dynamic Memory Management & Deep Copying** (`p.cpp`)
Implements proper dynamic memory allocation and deallocation with deep copying. The `Person` class allocates memory for string data, and the `Student` derived class adds its own allocated memory. Both classes implement destructors to prevent memory leaks by properly cleaning up allocated resources.

#### 7. **Struct Definition & Pointer Operations** (`substitution.cpp`)
Introduces C++ structs and demonstrates struct usage with pointers. A `Time` struct encapsulates hour, minute, and second values. The program shows struct variable declaration, initialization, pointer declaration, and passing structs as function parameters.

#### 8. **Virtual Inheritance & Diamond Problem Solution** (`x.cpp`)
Solves the "diamond problem" that occurs in multiple inheritance using virtual inheritance. When both `Midl` and `Mid2` virtually inherit from `Base`, the `Final` class receives only one copy of the `Base` class instead of two, preventing ambiguity and duplicate state.

#### 9-10. **Empty Files** (`i.cpp`, `z.cpp`)
Placeholder files for additional exercises or future implementations.

## Programming Concepts Covered

- **Inheritance Hierarchies**: Single and multiple inheritance patterns
- **Constructors & Destructors**: Initialization and cleanup in inheritance chains
- **Access Control**: Private, protected, and public member visibility
- **Static Members**: Class-level variables shared across instances
- **Dynamic Memory**: Heap allocation with `new` and `delete`
- **Pointers & References**: Pointer usage in object-oriented design
- **Method Overriding**: Reimplementing methods in derived classes
- **Initializer Lists**: Calling parent constructors in derived class constructors
- **Virtual Inheritance**: Resolving multiple inheritance conflicts

## Compilation & Execution

Each `.cpp` file is a standalone program and can be compiled independently:

```bash
g++ -o HW6 HW6.CPP
./HW6

g++ -o c c.cpp
./c

g++ -o code code.cpp
./code

# ... and so on for each file
