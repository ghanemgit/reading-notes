# Maps, primitives, File I/O

## Primitives VS objects

### In java the variables has two type, first type is primitive (Like int,boolean,...etc) and the other is reference type(Like Integer,Boolean,..etc).

### Autoboxing represent the process of comverting primitive type to a reference type.
### The benifits from used the primitive instead of refernce (Object type) is to save the memory.
### By using the premitive type except long and double we save our memory especially if we take the arrays as example.

## Ecxeption
### What is an exception? 
### An exception is an event which occurs during the execution of a program that disrupts the normal flow of the program instruction.
### Imagine that we have an error inside method at runtime system this method create an objext represent that error and contain more info about the error(thats call throwing an exception).
### If we have a code probably contain an error we have to enclose it by try and cath statement.
### Exception kinds:
### 1) Checked exception.
### A type of exception that can be excepted and the appropriate handling.
### 2) Error
### this exception condtions that are external to the applicatoin usually cannot recover from(ex: error related to hardware).
### 3) Runtime exception
### The condtion of this exception is usually internal the program and usualy program cannot anticipate(ex:logic error).

## Catching and handling exceptions
### Here will learn more about using the try, catch and final statements When executing Java code, different errors can occur: coding errors made by the programmer, errors due to wrong input, or other unforeseeable things.When an error occurs, Java will normally stop and generate an error message. The technical term for this is: Java will throw an exception (throw an error).
### The try statement allows you to define a block of code to be tested for errors while it is being executed. The catch statement allows you to define a block of code to be executed, if an error occurs in the try block.And The finally statement lets you execute code, after try...catch, regardless of the result.

## Scanning
### Scanner objext are useful for breaking down formated input into token and translating individula token according to their data type.and used to get user input from different souecce ike stream,users,files,etc.
  
