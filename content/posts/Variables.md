---
title: JavaScript - "Variable"
date: "2019-07-05"
template: "post"
draft: false
slug: "/javascript/variables/"
category: "JavaScript"
tags:
  - "JavaScript"
  - "Web Development"
description: "Here in the example, a is the variable in which we are storing the value 5, same as in b we are storing 6 then we perform sum and store in c variable."
---

Most of the time we need to store some values in programs. For example, if you need to add two numbers and take values from the user. For that, we need to store values in variables for having access in the future.

### _For Example :-_

```Js
var a = 5;
var b = 6;
var c = a + b;
console.log(c); //11
```

Here in the example, a is the variable in which we are storing the value 5, same as in b we are storing 6 then we perform sum and store in c variable. Variables are also used in storing strings, objects, etc. The declared variable is created before the execution of any code.

### _Types of variables:-_

There are three different types of variable declaration:-

- `var`
- `let`
- `const`

## **Variable — “var”:-**

`var` declaration, wherever they occur, are processed before any code is executed.

The scope of a variable declared with `var` is its current execution context, which is either the enclosing function or, for variables declared outside any function, global. If you re-declare a JavaScript variable, it will not lose its value.

### _Syntax:-_

```js
var varname1 [= value1] [, varname2 [= value2] ... [, varnameN [= valueN]]];
```

- Declared variables are constrained in the execution context in which they are declared. Undeclared variables are always global.

### _For Example :-_

```js
function x() {
  y = 1; // Throws a ReferenceError in strict mode.
  var z = 2;
}
x();
console.log(y); // 1
console.log(z); // Throws a ReferenceError: z is not defined outside x.
```

## **Variable — “let”:-**

ES2015 introduced two important keywords in JavaScript: ‘let’ and ‘const’. These two keywords provide Block Scope variables and constants in JS.

### _Syntax:-_

```js
let var1 [= value1] [, var2 [= value2]] [, ..., varN [= valueN];
```

### _For Example :-_

```js
let user = "John";
let age = 25;
let message = "Hello";
```

we can also declare like this in multiple lines:-

```js
let user = "John",
  age = 25,
  message = "Hello";
```

Technically both ‘var’ and ‘let’ do the same things. So, it depends upon personal taste.

## **Variable — “const”:-**

Constants are block-scoped, much like variables defined using the ‘let’ statement. The value of a constant cannot change through reassignment, and it can't be redeclared.

### _Syntax:-_

```js
const name1 = value1 [, name2 = value2 [, ... [, nameN = valueN]]];
```

### _For Example :-_

```js
const number = 42;
try {
  number = 99;
} catch (err) {
  console.log(err);
  // expected output: TypeError: invalid assignment to const `number’
  // Note — error messages will vary depending on browser
}
console.log(number);
// expected output: 42
```

A constant cannot share its name with a function or a variable in the same scope.

### _Case Sensitive:-_

Variables named ‘apple’ and ‘Apple’ are two different variables.
