# Inheritance and Interfaces

## Inheritance 

#### When a class is declared, with its specification, and the other sub-class members will want to use its member methods (functions); that’s when they will go for inheritance concepts. Inheritance in Java is a process of acquiring all the behaviours of a parent object.
### What is Inheritance in Java?
### Inheritance in Java Definition:
#### Inheritance in Java is a concept that acquires the properties from one class to other classes; for example, the relationship between father and son. In Java, a class can inherit attributes and methods from another class. The class that inherits the properties is known as the sub-class or the child class. The class from which the properties are inherited is known as the superclass or the parent class. In Inheritance, the properties of the base class are acquired by the derived classes.

### Extends keyword in Java
#### The extended keyword extends a class and is an indicator that a class is being inherited by another class. When you say class B extends a class A, it means that class B is inheriting the properties(methods, attributes) from class A. Here, class A is the superclass or parent class and class B is the subclass or child class.

### Types of Inheritance in Java
#### The different types of Inheritance are:

- Single Inheritance
- Multiple Inheritance
- Multi-Level Inheritance
- Hierarchical Inheritance
- Hybrid Inheritance



## Interfaces

#### An interface is a reference type in Java. It is similar to class. It is a collection of abstract methods. A class implements an interface, thereby inheriting the abstract methods of the interface.

#### Along with abstract methods, an interface may also contain constants, default methods, static methods, and nested types. Method bodies exist only for default methods and static methods.

#### Writing an interface is similar to writing a class. But a class describes the attributes and behaviors of an object. And an interface contains behaviors that a class implements.

#### Unless the class that implements the interface is abstract, all the methods of the interface need to be defined in the class.

### An interface is similar to a class in the following ways −

- An interface can contain any number of methods.

- An interface is written in a file with a .java extension, with the name of the interface matching the name of the file.

- The byte code of an interface appears in a .class file.

- nterfaces appear in packages, and their corresponding bytecode file must be in a directory structure that matches the package name.

### Declaring Interfaces
#### The interface keyword is used to declare an interface. Here is a simple example to declare an interface.
![image](https://user-images.githubusercontent.com/97638932/156459028-3f77640b-a908-425f-b455-34cbc03e66c2.png)
