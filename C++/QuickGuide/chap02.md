# Chapter 02. Compilers and Tools

# Compilers

This section mentions some of the most widely-used C++ compilers.

## GCC

GCC is one of the most common C++ compiler. It is an open source compiler which is installed by default on most Linux distro. GCC has different versions for different operating systems.

A single cpp file, for example, `main.cpp`, can be compiled using the following command in the terminal:

```
g++ main.cpp -o main
```

To run the program in the UNIX terminal, use the following syntax:

```
./main
```

To compile with newer version of C++, such as C++11, C++14, or C++17, add a flag in the compiling command:

```
g++ -std=c++17 main.cpp -o main
```

Also, you want to enable warnings to catch unwanted errors when running the program.

```
g++ -std=c++17 -Wall -Wextra main.cpp -o main
```

## Clang

Clang is another common C++ compiler which belongs to the LLVM Open Source Project.

## Visual C++

Visual C++ comes with the Visual Studio IDE on Windows. This compiler is developed by Microsoft and targets the Windows OS only.


# Tools

To program in C++, basically there are only two things you need:
* A compiler
* A text editor

If you have just started with C++, I would recommend **using a text editor**. Here are the reasons:
* It forces you to remember the syntax of the language. Most IDEs come with autocompletion. Over-relying on autocompletion makes it harder to remember the syntax.
* It forces you to use the terminal. Using the terminal is one of the most important skills for a programmer.
* It is light-weight, of course.

However, text editors are not always great. You will need a good IDE if:
* **you are lazy, you just want to grab the language as fast as possible and you do not want to mess with the terminal.**
* you need to work on a project.
* you need to debug a lot. A common scenario is when you need to implement some kind of data structure using pointers.


## Text editors

Some good text editors are:

* Atom: free, simple, beautiful, easy to use, and comes with a lot of powerful plugins.
* VSCode: pretty much similar to Atom. The user-interface is a bit closer to an IDE compared to Atom.
* Sublime Text: similar to Atom, but even better because it is super fast. The only downside is that it is NOT free.
* Notepad++ (Windows only): pretty standard text editor for coding
* Geany (Linux only): pretty standard text editor for coding
* Vim: has a learning-curve: using it is hard, and setting it up is even harder. You need a lot of time to get used to it, but once you are, you cannot live without it. I use Vim personally.


## IDEs

1. CLion: best C++ IDE in my opinion: easy to use, easy to debug, super powerful and super smart. It is not free, unfortunately, but if you are a student, you can use it for free by registering for a student license. All you need is an email with the domain of your institution.
2. Code::Blocks: nice IDE, but it has become quite obsolete nowadays. Not very smart. Debugging is not very well-supported.
3. Visual Studio: classic C++ IDE, but can only be used on Windows. Somewhat slow and resource-intensive. Visual Studio: classic C++ IDE, but can only be used on Windows. Somewhat slow and resource-intensive.
