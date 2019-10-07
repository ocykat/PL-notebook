# Chapter 5: Objects

## Objects

An object is a set of key-value pairs of data.

Object literal:
```js
var john = {
    firstName: 'John',
    lastName: 'Smith',
    birthYear: 1990
}
```

## Properties

To access a property of an objects, there are two different ways: dot notation and square-bracket notation.

```js
console.log(john.firstName);
console.log(john['firstName']);
```

## Methods

An object can contain functions. Function inside an object are called methods.

To use other properties of the same object inside a method, we need to use `this.propertyName`.

```js
var john = {
    firstName: 'John',
    lastName: 'Smith',
    birthYear: 1990,
    getAge: function() {
        return 2019 - this.birthYear;
    }
}

console.log(john.getAge());
```