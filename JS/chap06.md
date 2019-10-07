# Chapter 6: Execution Contexts

## Execution Context

A **Execution Context** is like a box/container/wrapper that stores variables and in which code is evaluated and executed.

The outermost execution context is called **Global Execution Context**. Any code that is not inside any function is in Global Execution Context.

Each execution context is associated with an **Execution Context Object**. For example, the Global Execution Context is associated with the `window` object.

```js
var a;
a === window.a; // true
```

Each **function call** has its own execution context.

All execution contexts create something called the **Execution Stack**.


## Execution Context Object

### Properties
Each Execution Context Object of a function contains 3 properties:

* Variable Object (VO): contains function arguments, inner-variable declarations, and function declarations.
* Scope chain: contains current VO, as well as all VOs of its parents. 
* `this` variable

### Phases

1. Creation Phase
* Creation of the VO
* Creation of the scope chain
* Determine the value of `this` variable

2. Execution Phase

The code of the function that generated the current execution context is ran line by line.

### The Variable Object

Steps of creation of a VO:

* The argument object is created, containing all the arguments that were passed into the function.
* For each inner function, a property pointing to the function is created.
* For each variable, a property is created and set to `undefined`.

The last 2 steps are called **hoisting**. Hoisting always happens **before** code starts executing.

Difference between function hoisting and variable hoisting:
* Functions are already defined before the execution phase starts.
* Variables are set to `undefined` before the execution phase starts. Variables can only become defined in the execution phase.