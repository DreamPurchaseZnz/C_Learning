# C++ learning tutorial


## Reference
[C++ tutorial](http://www.cplusplus.com/doc/tutorial/)
[Programming in C](https://www.hermetic.ch/cfunlib.htm)


## [The Use of * and & in C/C++](https://www.hermetic.ch/cfunlib/ast_amp2.htm)
### The use of * in C
```
(a)   Multiplication:   x = y*z;
(b)   Multiply-assign:   x *= y;   Means the same as: x = x*y;
(c)   Comments:   /* your comment here */
(d)   Pointer declarations:   int *p; or int* p;   Read: p is a pointer to an int.
(e)   Compound pointers:   int **p; or int** p;   Read: p is a pointer to a pointer to an int. 
      (Also int ***p; and so on.)
(f)   De-referencing:   x = *p;   Read: Assign to x the value pointed to by p.
```

### The use of & in C
```
(a)   Logical-and:   if ( ( a>1 ) && (b<0) ) ...
(b)   Bitwise-and:   x = a&b;   Corresponding bits are and'ed (e.g. 0&1 -> 0)
(c)   Bitwise-and-assign:   x &= y;   Means the same as: x = x&y;
(d)   Address-of operator:   p = &x;   Read: Assign to p (a pointer) the address of x.
```
### The additional use of & (in parameters) in C++

C++ uses a type of variable called a "reference" variable (or simply a "reference") which is not available in C (although the same effect can be achieved using pointers).

References, pointers and addresses are closely related concepts. Addresses are addresses in computer memory (typically the address in memory where the value of some variable is stored), e.g. (in hexadecimal) 0xAB32C2. Pointers are variables which hold addresses, and so "point to" memory locations (and thus to the values of variables). Conceptually, reference variables are basically pointers by another name (but may not be instantiated as such by the compiler).

It is possible to declare a reference within a function, like other variables, e.g.
```
void main(void) 
{ 
int i; 
int& r = i; 
...
}
```
but this is pointless, since the use of the reference is equivalent to the use of the variable it references.

References are designed to be used as parameters (arguments) to functions, e.g.
```
#include <iostream.h>

void f(int& r);

void main(void) 
{ 
int i=3;

f(i); 
cout << i; 
}

void f(int& r) 
{ 
r = 2*r; 
}
```



## structure of C++ Language

These tutorials explain the C++ language from its basics up to the newest features introduced by C++11. Chapters have a practical orientation, with example programs in all sections to start practicing what is being explained right away.
```
Introduction
Compilers

Basics of C++
Structure of a program
Variables and types
Constants
Operators
Basic Input/Output

Program structure
Control Structures
Functions
Overloads and templates
Name visibility

Compound data types
Arrays
Character sequences
Pointers
Dynamic Memory
Data structures
Other data types

Classes
Classes (I)
Classes (II)
Special members
Friendship and inheritance
Polymorphism

Other language features
Type conversions
Exceptions
Preprocessor directives

C++ Standard Library
Input/Output with files
```
## Compiler

Computers understand only one language and that language consists of sets of instructions made of ones and zeros. This computer language is appropriately called machine language.

Because a computer can only understand *machine language* and humans wish to write in *high level languages* and high level languages have to be re-written (translated) into machine language at some point. 

This is done by special programs called *compilers*, interpreters, or assemblers that are built into the various programming applications.

## Console programs
Integrated Development Environment (IDE)

 An IDE generally integrates several development tools, including *a text editor* and *tools to compile programs directly from it*.
 






