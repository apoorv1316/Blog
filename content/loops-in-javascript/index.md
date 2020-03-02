---
title: "Loops In Javascript"
description: "Loops are used to execute the same block of code again and again, as long as a certain condition is met. The basic idea behind a loop is…"
date: "2020-02-24T03:26:14.627Z"
categories: []
published: true
canonical_link: https://medium.com/@tiwari.apoorv1316/loops-in-javascript-905dc3687f8b
redirect_from:
  - /loops-in-javascript-905dc3687f8b
---

Loops are used to execute the same block of code again and again, as long as a certain condition is met. The basic idea behind a loop is to automate the repetitive tasks within a program to save time and effort. Suppose you want to type a ‘Hello world’ message 20 times on your webpage. Of course, you will have to copy and paste the same line 20 times. Instead, if you use loops, you can complete this task in just 3 or 4 lines.

### Different Types of Loops

There are mainly four types of loops in JavaScript.

1.  for loop
2.  for/in a loop
3.  while loop
4.  do…while loop

### while loop

The `while` loop loops through a block of code as long as the specified condition evaluates to true. As soon as the condition fails, the loop is stopped. The JavaScript while loop _iterates the elements for the infinite number of times_. It should be used if the number of iteration is not known. The syntax of while loop is given below.

```
while(condition)

{

lines of code to be executed

}
```

### for loop

The `for` loop repeats a block of code as long as a certain condition is met. It is typically used to execute a block of code for certain number of times.Its syntax is:

```
for(initialization; condition; increment) {
    // Code to be executed
}
```

The parameters of the `for` loop statement have the following meanings:

-   **_initialization_** — it is used to initialize the counter variables and evaluated once unconditionally before the first execution of the body of the loop.
-   **_condition_** — it is evaluated at the beginning of each iteration. If it evaluates to `true`, the loop statements execute. If it evaluates to false, the execution of the loop ends.
-   **_increment_** — it updates the loop counter with a new value each time the loop runs.

### do…while loop

The JavaScript do-while loop _iterates the elements for the infinite number of times_ like while loop. But, code is _executed at least_ once whether the condition is true or false. The generic syntax of the do-while loop is:

```
do {
    // Code to be executed
}
while(condition);
```

### for…in loop

The for-in loop is a special type of a loop that iterates over the properties of an object, or the elements of an array. The generic syntax of the `for-in` loop is:

```
for(variable in object) {
    // Code to be executed
}
```

The loop counter i.e. _variable_ in the for-in loop is a string, not a number. It contains the name of the current property or the index of the current array element.
