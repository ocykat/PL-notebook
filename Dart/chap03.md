# Chapter 3: Operators

There are 7 types of operators:
* Arithmetic
* Assignment
* Relational
* Type-Test (*)
* Logical
* Condidtional
* Bitwise

## Arithmetic Operators

| Operator        | Name/Meaning                                 |
| --------------- | -------------------------------------------- |
| `c = a + b`     | Addition                                     |
| `c = a - b`     | Subtraction                                  |
| `c = -a`        | Unary Minus                                  |
| `c = a * b`     | Multiplication                               |
| `c = a / b`     | Division                                     |
| `c = a ~/ b`    | Floor Division                               |
| `c = a % b`     | Euclidean Modulo (result is always positive) |
| `a++` and `++a` | Increment                                    |
| `a--` and `--a` | Decrement                                    |

```dart
void main() {
    print(" 5  /  4 = ${5 / 4}");
    print(" 5 ~/  4 = ${5 ~/ 4}");
    print("-5  %  4 = ${-5 % 4}");

    int a = 0;
    int b = 0;
    print("Pre-increment a   : a = ${++a}");
    print("Post-increment b  : b = ${b++}");
    print("After incrementing: a = ${a}, b = ${b}");
}

/*
======= OUTPUT =======
 5  /  4 = 1.25
 5 ~/  4 = 1
-5  %  4 = 3
Pre-increment a   : a = 1
Post-increment b  : b = 0
After incrementing: a = 1, b = 1
*/
```


## Assignment Operators

| Operator  | Name/Meaning                                              |
| --------- | --------------------------------------------------------- |
| `a += b`  | Addition & Assignment                                     |
| `a -= b`  | Subtraction & Assignment                                  |
| `a *= b`  | Multiplication & Assignment                               |
| `a /= b`  | Division & Assignment                                     |
| `a ~/= b` | Floor Division & Assignment                               |
| `a %= b`  | Euclidean Modulo * Assignment (result is always positive) |
| `a ??= b` | Assign the value of `b` to `a` **only if `a` is null**    |


## Relational Operators

| Operator | Name/Meaning             |
| -------- | ------------------------ |
| `a < b`  | Less than                |
| `a <= b` | Less than or equal to    |
| `a > b`  | Greater than             |
| `a >= b` | Greater than or equal to |
| `a == b` | Equal                    |
| `a != b` | Not equal                |


# Type-Test Operator

| Operator  | Name/Meaning                                                  |
| --------- | ------------------------------------------------------------- |
| `a is X`  | is: returns `true` if `a` is of type X, `false` otherwise     |
| `a is! X` | is not: returns `false` if `a` is of type X, `true` otherwise |


## Logical Operators

| Operator | Name/Meaning |
| -------- | ------------ |
| `&&`     | AND          |
| `||`     | OR           |
| `!`      | NOT          |


## Conditional Operators

| Operator           | Name/Meaning                                         |
| ------------------ | ---------------------------------------------------- |
| `a = cond ? x : y` | if `cond` is `true`, returns `x`; else, returns `y`  |
| `a = x ?? y`       | if `x` is not `null`, returns `x`; else, returns `y` |


## Bitwise Operators

| Operator | Name/Meaning                                         |
| -------- | ---------------------------------------------------- |
| `a & b`  | Bitwise AND                                          |
| `a | b`  | Bitwise OR                                           |
| `a ^ b`  | Bitwise XOR                                          |
| `~ a`    | Bitwise NOT                                          |
| `a << b` | Left shift: `a` is shifted by `b` bits to the left   |
| `a >> b` | Right shift: `a` is shifted by `b` bits to the right |
