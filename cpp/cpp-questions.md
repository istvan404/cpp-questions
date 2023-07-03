# List of C++ questions for interviews.

## Table of content

...

## Introduction

### What is a C++? What are the advantages of C++?

C++ is a multi-paradigm programming language supporting object-oriented, imperative, functional and other programming styles.

Advantges of C++ are:
- multi-paradigm language
- no garbage collection
- efficient and fast

### What is the difference between C and C++?

C is a procedural, function-driven proramming language, it does not support OOP conecpts like polymorphism, data abstraction, classes and objects.

C++ is a multi-paradigm language which was introduced as an improved version of C with OOP and other programming style capabilities. It also support operator and function overloading.

### What are files with .cpp, .hpp and .h extensions?

The C language uses .h header files, while C++ can use .h and .hpp as header files.
The .cpp files are the source files, after the compiler finished with the preprocessor, this file becomes a compilation unit.

### What are the stages of a c++ program's compilation? Explain each stage

##### 1. Preprocessing

The preprocessor handles the preprocessor directives, like #include and #define.
The output of the preprocessor is a "pure" C++ file without any preprocessor directives, called a compilation unit.

##### 2. Compilation

The compilation is performed on each compilation unit of the preprocessor.
The compiler parses the pure c++ code and converts it into and object file with .o extension.

Most compilers let you stop compilation at this point. This lets you compile each source code separately, without the need to recompile everything.

##### 3. Linking

The linker is what creates the final executable.
It linkes all the object files and libraries by replacing the references to undefined symbols with the correct address.

### What is the difference between a declaration and definiton?

Declaration introduces an identifier and describes it's type, be it a type, object, or a function. A declaration is whate the compiler needs to accept references to that identifier.

Definition instantiates/implements this identifier. It is what the linked needs in order to link references to those entities.

An identifier can be declared as often as you want, however, it mus be defined exactly once.


## Types
## Functions
## Pointers and References

### What is a pointer?

A pointer is a variable that stores the memory address of an object.
It has to have a type.
It's value can be reassigned or it can hold a null value (`nullptr` / `null`).
To access the memory location of the pointer, we have to dereference it with `*`.
To access a variable's memory address, we have to use `&`.

```
int my_variable = 8;
int *p = &my_variable;
```

### What is a reference?

A reference is essentially a constant pointer. With syntactic sugare we can replace `* const` with `&`.
A reference can't have null value and it can't be reassigned.

```
void swap( int* const a, int* const b )
void swap( int &a, int &b )
```


### What is the difference between a pointer and a reference?



## Classes