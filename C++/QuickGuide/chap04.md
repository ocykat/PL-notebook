# Chapter 04. Input/Output

This chapter shows how to read input from the console and print output to the console in C++.

## Printing Output

To write output to the console, we use the `cout` object together with the `<<` operator.  In the last chapter, we got to know about `cout` already.

You can print multiple things within only one statement like this:

```cpp
cout << "This " << "is " << "a " << "sentence." << '\n';
```

Beside printing strings of text, we can also print values of variables.

```cpp
int a;
double b;
char c;

// do something...

cout << a << b << c;
```

## Reading Input

In C++, to read input, we use the `cin` object, which also belongs to the `<iostream>` library, together with the `>>` operator.

```cpp
int a;
cin >> a;
```

In the code above, `cin` is used to read an integer and assign that integer to the variable `a`.

We can also read multiple things within one statement:

```cpp
int a;
double b;
char c;
cin >> a >> b >> c;
```
