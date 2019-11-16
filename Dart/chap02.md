# Chapter 2: Data Types, Variables and Literals

## Data types
### Numbers [*]
 Numbers represent numeric literals.
  * Integer - keyword: `int`
  * Double - keyword: `double`

### Strings [*]
* Strings represent sequences of characters.
* Keyword: `String`
* A Dart string is a sequence of **UTF-16 code units**. Sequences of *UTF-32 code units* can be represented by *runes*.

### Boolean [*]
* Keyword: `bool`
* Literals: `true` and `false`

### Collections: List and Map
The Dart core library enables creation and manipulation of these collections through the predefined List and Map classes respectively.

#### List [*]
* A **List** is an ordered group of objects.
* Equivalent to (kind of):
  * array/`std::vector` in C++
  * array/`ArrayList` in Java
  * list in Python.

#### Map [**]
* A **Map** data type represents a set of values as key-value pairs.
* Equivalent to (kind of):
  * `std::map`/`std::unordered_map` in C++
  * `TreeMap/HashMap` in Java
  * dictionary in Python

### Dynamic Type [*]
* Dart is an **optionally-typed language**: If the type of a variable is not explicitly specified, the variable’s type is dynamic.
* The `dynamic` keyword can also be used as a type annotation explicitly.


## Variables and Values (Literals)
### Type of a variable [*]
* Every value (literal) has a type.
* Every variable has a type it can *reference*. (a variable is in fact a pointer)
* Once a variable as a type associated, its type cannot be changed.

```dart
var name = "John Doe";
name = 123;            // error
```
* We do not have to annotate types, since Dart can guess!

### Static Types vs Dynamic Type [**]
* Avoid Dynamic Type! Why? Because using static types results in:
  * better performance
  * ease of debugging
  * better code maintainability
  * simpler unit testing

### Declaration and Initialization [*]

After **declaration**, the default value of any variable **of any type** is `null`.

```dart
void main() {
  var x;     // Declaration only
  var y = 1; // Declaration + Initialization

  print("x = ${x}");
  print("y = ${y}");
}

/**
====== OUTPUT ======
x = null
y = 1
```