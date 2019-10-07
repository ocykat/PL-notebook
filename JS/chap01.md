# Chapter 1: Variables

## Primitive Data Types

| Data Type | Description                                                  |
| --------- | ------------------------------------------------------------ |
| Number    | All floating-point numbers                                   |
| String    | Literals can be single-quoted or double-quoted               |
| Boolean   |                                                              |
| Undefined | Data type of a variable that has not been assigned any value |
| null      | We know what it is and what it does                          |

## Variable Coercion

```js
var age = 28;
var isStudent = true;
console.log("I am " + 28 + " and am I a student? " + isStudent);
```

First, the values of `age` and `isStudent` is converted into String. Then, the strings are concatenated.

## Variable Mutation

In JavaScript, we can change the data type of a variable.

```js
var age = 28;
age = "twenty-eight"; // this is allowed
```