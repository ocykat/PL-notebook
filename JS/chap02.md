# Chapter 2: Operators

<!-- There are 7 types of operators:
* Arithmetic
* Assignment
* Relational
* Type-Test (*)
* Logical
* Condidtional
* Bitwise -->

## Arithmetic Operators [*]

| Operator        | Name/Meaning                                 |
| --------------- | -------------------------------------------- |
| `c = a + b`     | Addition                                     |
| `c = a - b`     | Subtraction                                  |
| `c = -a`        | Unary Minus                                  |
| `c = a * b`     | Multiplication                               |
| `c = a / b`     | Division                                     |
| `c = a ** b`    | Exponentiation (ES2016)                      |
| `c = a % b`     | Euclidean Modulo (result is always positive) |
| `a++` and `++a` | Increment                                    |
| `a--` and `--a` | Decrement                                    |


## Assignment Operators [*]

| Operator | Name/Meaning                                              |
| -------- | --------------------------------------------------------- |
| `a += b` | Addition & Assignment                                     |
| `a -= b` | Subtraction & Assignment                                  |
| `a *= b` | Multiplication & Assignment                               |
| `a /= b` | Division & Assignment                                     |
| `a %= b` | Euclidean Modulo * Assignment (result is always positive) |


## Relational Operators [*]

| Operator  | Name/Meaning                   |
| --------- | ------------------------------ |
| `a < b`   | Less than                      |
| `a <= b`  | Less than or equal to          |
| `a > b`   | Greater than                   |
| `a >= b`  | Greater than or equal to       |
| `a == b`  | Coercion + Equality            |
| `a === b` | Equality (both Type and Value) |
| `a != b`  | Not equal                      |


## `typeof` Operator [*]

| Operator   | Name/Meaning                          |
| ---------- | ------------------------------------- |
| `typeof a` | returns the data type of variable `a` |


## Logical Operators [*]

| Operator                  | Name/Meaning |
| ------------------------- | ------------ |
| `&&`                      | AND          |
| <code>&#124;&#124;</code> | OR           |
| `!`                       | NOT          |


## Conditional Operators [**]

| Operator           | Name/Meaning                                        |
| ------------------ | --------------------------------------------------- |
| `a = cond ? x : y` | if `cond` is `true`, returns `x`; else, returns `y` |


## Bitwise Operators [**]

| Operator                | Name/Meaning                                         |
| ----------------------- | ---------------------------------------------------- |
| `a & b`                 | Bitwise AND                                          |
| <code>a &#124; b</code> | Bitwise OR                                           |
| `a ^ b`                 | Bitwise XOR                                          |
| `~ a`                   | Bitwise NOT                                          |
| `a << b`                | Left shift: `a` is shifted by `b` bits to the left   |
| `a >> b`                | Right shift: `a` is shifted by `b` bits to the right |
