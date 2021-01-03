# Programming Methodology #4
## History of Computing

The first computing device was invented about 4000 years ago: abacus.

The progress of computing had then stalled for thousands of years. In around 1800, Charles Babbage designed two computing devices by mechanical means: the difference engine and the analytic engine. These engines are designed to be powered by steam to perform automatic calculation. However, Charles Babbage did not live long enough to realize his design.

People already started programming well before the invention of programmable devices, these programmers anticipated the future of computing and started writing programs for computers that did not exist. They then simulate these programs by hand.

Ada Byron, the daughter of Lord Byron was the first programmer in the world.

When the first computing device was created, they use cards punched with holes to read instructions.

The first computing prototypes were created during the 1930s.

In 1946, the first large scale electromagnetic computer – ENIAC, was created.

In 1971, the first microprocessor – Intel 4004, was created.

## Computer Science and Programming
Computer science is the study of problem solving with computers (or computational methods). Programming is just an artifact to realize this process.

## The Hierarchy of Programs
Computers only understand binaries, which is a combination of 0s and 1s. Thus, the machine languages have to be coded in 0s and 1s.

In order to simplify the process of programming, high-level languages are invented: C, C++, Java, etc.

In order to translate high-level languages into machine languages, the code has to go through compilers. This process is called compilation.

In the compilation process, the high-level code is also called **source code**, while the low-level instructions are called **object code**.

While the source code is usually platform independent, the object code has to be written specifically to a certain type of machines. Thus, compilers are platform dependent.

### Java is a Special Case
Java programs are platform independent. This is achieved by running the programs through a virtual machine (Java Virtual Machine, JVM).

Java source code is compiled into a special intermediate code called Java byte code and encapsulate into Java class files.

These files are then run on the JVM, where the intermediate language is then interpreted on-the-fly by the JVM.

## Object-oriented Programming
Object-oriented programming is a way of creating program based on encapsulation of behaviors and data. These encapsulations are achieved using a set of classes.

### Class Hierarchy
A class is a set of methods and data. They can be extended to fit different purposes.

If a class extends another class, the former is called the subclass while the latter is called the superclass. The subclass has all the methods and data of the superclass, this characteristic is called inheritance.

In general, superclasses are more general classes, where subclasses have more specific methods and data.

You can use a biology tree as an analogy to the class hierarchy.

### Relationship between Classes and Instances
An object is an instance of a class. There can be many instances sharing a same class. Each instance is different from other instances.

In a sense, classes are the "templates" of objects.

## The ACM Library
### The ACM Program Hierarchy
ACM is a graphical user interface library in Java, developed in Stanford University.

The ACM has a program hierarchy as shown below:
Applet -> JApplet -> Program -> Console/Dialog/Graphics Program

A typical Java library import command:
```
import acm.graphics.*
import acm.program.*

```

### Graphics Program
The `GraphicsProgram` is a UI library in Java, it uses a collage model with blank canvas to create UIs.

#### Frequently Used Methods:
`GLabel()`: Graphics Labels, used to display texts.
`GRect()`, `GOval()`, `GLine()`, etc.: 
`add()`: Add, display instances into the canvas.

### Console Program
`println()`:
`readInt()`:

### Dialog Program

