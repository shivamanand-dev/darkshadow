---
title: JavaScript - "Code Structure"
date: "2019-07-03"
template: "post"
draft: false
slug: "/javascript/code-structure/"
category: "JavaScript"
tags:
  - "JavaScript"
  - "Web Development"
description: "It doesn’t matter if you are coding anything like HTML, CSS, JavaScript, Java, or any other kind of code. There is a structure to write every code and that is the building blocks of code."
---

It doesn’t matter if you are coding anything like HTML, CSS, JavaScript, Java, or any other kind of code. There is a structure to write every code and that is the building blocks of code.

# **What actually is Code Structure?**

So, I will use HTML for illustration purposes of code structure it will be easy to understand. You can call it a design and flow of a document.

### _For Example :-_

```html
<!DOCTYPE html>
    <head>
        <title></title>
    </head>
    <body>
        <div>
            <h1></h1>
        </div>
    </body>
</html>
```

Here in the above example, you are to determine a clear outline of the document and where your code should go.

If anyone code likely that it is horrible to receive the code like the following and asked to fix it….

```html
<!DOCTYPE html> <head> <title> </title> </head> <body> <div> <h1> </h1> </div> </body> </html>
```

It takes very long to understand the code that what this is actually and where is an error. So we write code which is easily understandable.

# **Why Code Structure?**

Have you ever read an article or anything where there are no punctuation marks? You weren’t able to make sense of it you will have a problem finding where the sentence is ending or from where the new line starts. It's same with coding.

What in the first example if any developer is reading your code they can quickly scan your code and find the problems.

And in the second example either he will say I’m sorry, I will not work with you or first, he has to work on your code. If the structure is clear and clean they may pick up on the issue immediately or tell you they will take a closer look later in the day.

## **Statements**

Statements are syntax constructs and commands that perform actions.

Here in JS statements can be separated using a semicolon.

### _For Example :-_

```js
alert("Hello");
alert("World");
```

Statements are written in separate lines to make the code more readable:-

```js
alert("Hello");
alert("World");
```

There are cases when a newline does not mean a semicolon. For example:

```js
alert(3 + 1 + 2);
```

The code outputs 6 because JavaScript does not insert semicolons here. It is obvious that if the line ends with a plus, "+" then it is an “incomplete expression”, so the semicolon is not required. And in this case that works as intended.
