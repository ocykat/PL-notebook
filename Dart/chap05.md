# Chapter 5: Loops

## `for` loop [*]

```dart
void main() {
  int sum = 0;
  for (int i = 1; i <= 5; i++) {
    sum += i;
  }
  print(sum);
}

/**
====== OUTPUT =======
15
*/
```


## `while` loop [*]

```dart
void main() {
  int sum = 0;
  int i = 0;
  while (sum < 100) {
    sum += i;
    i++;
  }
  print(sum);
}
```


## `do-while` loop [*]

```dart
void main() {
  int i = 2;
  do {
    print("${i} x ${i} = ${i * i}");
    i = i * i;
  } while (i < 100);
}
```


## Loop Control Statements [*]

Dart also offers the `break` and `continue` statements like a lot of other languages.


## Labels [**]

Label can be used to control the flow of a nested loop.

```dart
void main() {
  outerloop: for (int i = 0; i < 4; i++) {
    for (int j = 0; j < 4; j++) {
      print("i = ${i}, j = ${j}");
      if (i == j) {
        continue outerloop;
      }
    }
  }
}
/**
======= OUTPUT =======
i = 0, j = 0
i = 1, j = 0
i = 1, j = 1
i = 2, j = 0
i = 2, j = 1
i = 2, j = 2
i = 3, j = 0
i = 3, j = 1
i = 3, j = 2
i = 3, j = 3
*/
```