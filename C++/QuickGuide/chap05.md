# Chapter 05. Variables and Fundamental Data Types

## Variables

* C++ is a **strongly-typed** language, meaning every variable must have a certain data type when it is declared.

```cpp
int a;
char b;
```

* To assign value to a variable, use the `=` operator.

```cpp
int x = 10;
int y = 0;
```

## Fundamental Data Types

This part only mentions the most common data types. For more details, visit this [link](http://www.cplusplus.com/doc/tutorial/variables)

### Integer
| Type         | Size (byte) | Range                                |
|--------------|-------------|--------------------------------------|
| int          | 4           | -2^31 to 2^31 - 1 (2^31 ~ 2 * 10^9)  |
| long long    | 8           | -2^63 to 2^63 - 1 (2^63 ~ 9 * 10^18) |
| unsigned_int | 4           | 0 to 2^32                            |


### Double
| Type         | Size (byte) | Precision         |
|--------------|-------------|-------------------|
| float        | 4           |                   |
| double       | 8           | better than float |


### Character
| Type     | Size (byte) |
|----------|-------------|
| char     | 4           |
