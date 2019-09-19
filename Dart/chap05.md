# Chapter 5: Loops

## `for` loop

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

## `while` loop

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

## `do-while` loop

```dart
void main() {
  int i = 2;
  do {
    print("${i} x ${i} = ${i * i}");
    i = i * i;
  } while (i < 100);
}
```

## Loop Control Statements

Dart also offers the `break` and `continue` statements like a lot of other languages.