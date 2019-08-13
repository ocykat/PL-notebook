# Chapter 1: Basics of Dart: The Hello World Program & Printing


## The Hello World Program
```dart
void main() {
    print('Hello World');
}
```

A Dart program starts by entering the `void main()` function. (quite similar to many other languages)


## Printing

### The `print()` function

The `print()` function always automatically add a new line character. To avoid this, use the `stdout` object instead. (see below)

### String Interpolation

**String interpolation**: replace a variable (or the result of an operation) with the value stored by that variable.
* Note: always use curly braces just to be safe!

```dart
void main() {
    String name = "John";
    print("1. Hello $name");   // This runs fine but NOT recommended
    print("2. Hello ${name}"); // This is way better

    // Here's why
    print("3. Length of name is: $name.length");
    print("4. Length of name is: ${name.length}");

    // Operation can also be interpolated
    int a = 7;
    int b = 4;
    print("5. a - b = ${a - b}");
}

/*
========= OUTPUT =========
1. Hello John
2. Hello John
3. Length of name is: John.length
4. Length of name is: 4
5. a - b = 3
*/
```