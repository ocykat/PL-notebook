# Chapter 6: Lists

## Introduction

A **List** is an ordered group of objects.

The `List` class belongs to the `dart:core` library.

There are two types of `List` in Dart:
* Fixed-length lists: the size (number of elements) of the list CANNOT be changed once it is created
* Growable lists: the size of the list CAN be changed once it is created


## Declaration [*]

There are a couple of ways to **declare** a list.

```dart
// Fixed-length lists
var a = new List(4);  // the default value of each element is `null`
List b = new List(4);

// Growable lists
var c = new List();
List d = new List();

// These are also growable lists
var e = [1, 2, 3];
List f = [5, 6, 7];

// A list can contain different data types
List g = [1, "Hi"];

// We can restrict a list to contain only 1 data type
List<int> h = [1, 2, 3];
```

## Add an element to the list (growable lists only) [*]

To add an element to *the end* of a growable list, use the `add()` method.

```dart
void main() {
  List a = new List(2);
  print(a);
//   a.add(1); // can't do this
  
  List b = new List();
  b.add(1);
  b.add(2);
  print(b);
  
  List c = [3, 4];
  c.add(5);
  print(c);
}

/**
====== OUTPUT ======
[null, null]
[1, 2]
[3, 4, 5]
*/
```

## Access individual element in a `List` [*]

To access an individual element, use the `[]` operator.

```dart
void main() {
  List a = new List(2);
  a[0] = 2;
  a[1] = 3;
  print(a);
}

/**
======= OUTPUT =======
[2, 3]
*/
```

## Traverse through a `List` [*]

### `for` loop [*]

To get the size of a list, use the `length` property.

```dart
void main() {
  List a = [0, 7, 5, 2, 4];
  
  for (int i = 0; i < a.length; i++) {
    print("a[${i}] = ${a[i]}");
  }
}

/**
====== OUTPUT ======
a[0] = 0
a[1] = 7
a[2] = 5
a[3] = 2
a[4] = 4
*/
```

### `for-in` loop [**]

```dart
void main() {
  List a = [0, 7, 5, 2, 4];
  
  for (var x in a) {
    print("x = ${x}");
  }
}
/**
====== OUTPUT ======
x = 0
x = 7
x = 5
x = 2
x = 4
```

## The `List` class: constructors, properties, and methods [***]

For a more completed list, visit [here](https://api.dartlang.org/stable/2.4.1/dart-core/List-class.html).


### Static Methods

* To create a fixed-length list in which every element has the same value:
```dart
List flags = List.filled(4, false); // flags.length = 4
```


### Properties

| Property | Return                         |
| -------- | ------------------------------ |
| `length` | `(int)` the length of the list |


### Methods

#### Sort
* To sort a list, use the `sort()` method.

```dart
void main() {
  List a = [0, 7, 5, 2, 4];
  a.sort();
  print(a);
}
/**
====== OUTPUT ======
[0, 2, 4, 5, 7]
*/
```