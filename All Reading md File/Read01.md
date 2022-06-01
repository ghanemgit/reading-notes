# Java Language Basics

## Introduction to Java
### We will start introduction about Java by answering these questions, What is Java? Why java in 2022? and how to start using java?
### First Java is a programming language and platform first released by Sun Microsystems in 1995 , Beacause it since 95 now you may be wondering why java in 2022 I will tell you,the features that made the java language exist to this tome listed below:
- Simple language. 
- OOP language.
- High performance.
- Secure.
- Dynamic.
#### Can you read more about this features here => [The Java Language Environment](https://www.oracle.com/java/technologies/language-environment.html)
### In general you can use java by create java file that contain your code and then conver it to class file contain bytecodes(that able us to run progrm on different operating system) by using compiler(javac), after that bytecodes pass through Java virtual machine to convert it to binary code that computor understand it. 

## Variables
### Variables allow the java program to store values during the runtime of program,In general Java defines these kinds of variables:
- Instance variables(or non-static fields) : Instance because their value are unique to each instance of class.
- Class variable : there is exactly one copy of this variablein extence.
- Local variable : Temporary state(variable) stored in method.
- Parameters : are always classified as variable not fields.
### Now lets talk about two major type of varibles in Java:
1) Primitive data type : They're stored directly on the stack.
2) Non-primitive data types(reference type): Can be used to call methods to perform certain operations.
### The table* below illustrate the differnet types primitive data type.
![Primitive](https://user-images.githubusercontent.com/97638932/155844143-d0fbfa90-724d-4b8a-9933-b8182e23acbd.png)
[*Source](https://lessons2all.com/java_datatypes_operators.php)

## Operators
### Operators in Java are the special symbols that perform specific operations and then return a result.
### Types of Operators in Java are:
1. Arithmetic Operators.
2. Assignment Operators.
3. Auto-increment Operator and Auto-decrement Operators.
4. Logical Operators.
5. Comparison (relational) Operators.
6. Bitwise Operators.
7. Ternary Operator.

![image](https://user-images.githubusercontent.com/97638932/155844282-e926a09b-ba86-4d54-9f42-361d3fc46a50.png)

[Source](https://www.softwaretestingmaterial.com/wp-content/uploads/2018/03/Operators-Table.png)

## Expressions, Statements, and Blocks
### Java statements appear inside of methods and classes, they describe all activities of a Java program. Variable declarations and assignments, such as those in the previous section, are statements, as are the basic language structures like use of ++ or --, Method invocations, conditionals and loops. Expressions describe values, an expression is evaluated to produce a result, to be used as part of another expression or in a statement.
## Control Flow Statements
### Control flow statements let you control the flow of the execution of the code in your program. In Java programming language, you can control the flow of execution of the code by placing the decision making, branching, looping, and adding conditional blocks.
### Based on this, we can classify the types of control flow statements as follows:
1) Decision Making Statements.
2) Looping Statements.
2) Branching Statements.

![control flow statements](https://user-images.githubusercontent.com/97638932/155844806-6523ed5e-2079-4dbd-a496-fb5205eb3487.png)

[source](https://soshace.com/wp-content/uploads/2020/01/untitled-drawing.jpg)
### The if-then statement is the most basic of all the control flow statements. It tells your program to execute a certain section of code only if a particular test evaluates to true. The if-then-else statement provides a secondary path of execution when an "if" clause evaluates to false. Unlike if-then and if-then-else, the switch statement allows for any number of possible execution paths. The while and do-while statements continually execute a block of statements while a particular condition is true. The difference between do-while and while is that do-while evaluates its expression at the bottom of the loop instead of the top. Therefore, the statements within the do block are always executed at least once. The for statement provides a compact way to iterate over a range of values. It has two forms, one of which was designed for looping through collections and arrays.


