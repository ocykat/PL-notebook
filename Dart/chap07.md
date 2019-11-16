# Chapter 7: Functions

## Declaration [*]

The declaration of a function includes:

* The return type **(not required)**
* Function name
* Parameter list
  * Variable type **(not required)**
  * Variable name
* The function's body

```dart
void main() {
  print(sum(1, 2));
}

int sum(int a, int b) {
  return a + b;
}
```

The following is also fine:

```dart
main() {
  print(sum(1, 2));
}

sum(a, b) {
  return a + b;
}
```