# Read 05

## Comparison and logical operators


#### What's a flowchart ?

A flowchart is a diagram that depicts a process, system or computer algorithm, it rusually represents workflow or a process.

![flow chart](https://cacoo.com/wp-app/uploads/2019/09/basic-flowchart-template@2x.png)


### Comparison operators:
 You can compare one value in the script to another value that is expected; and the result should be boolean (true or false).
 <p>&nbsp;</p>

  - `==` : is equal to, compares two values (whether they are strings or numbers or boolean etc.)
 - `!=`  : is not equal to.
 - `===` :strictly equal to 
 - `!==` : strictly not equal to.
 <p>&nbsp;</p>

>strict method: means the data type and the values should be equal.

<p>&nbsp;</p>
What does evaluating the condition mean?
- testing or checking the condition.
<p>&nbsp;</p>

what is type coercion ?
Its the process of converting one data type to another.
<p>&nbsp;</p>

>> Because of type coercion all js values can be treated as true or false.
<p>&nbsp;</p>
<p>&nbsp;</p>


### What are ***Falsy Truthy values***?
- Falsy values are values that can be treated as false.
- Truthy values are values that can be treated as Truth.


### FALSY VALUES:
---


Value| Description 
---  | ----
var A=false:| the traditional false.
var a= 0; | the number zero.
var a=" "; | empty value
var a= 5/b;| NaN (NOT a NUMBER)
var a;| no value assigned

<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>

### TRUTHY VALUES:
---
Value | Description
---| ---
var a= truth;| the traditional truth
var a=1;| the number 1
var a="any string with content even if it was true or false";|string with content.
var a=10/5;| calculations

<p>&nbsp;</p>
<p>&nbsp;</p>

## LOOPS
___
They are used to check whether a condition makes true or not; if the condition is true they will run a code block then update the counter and check the condition again and run the program again if it was true.
<p>&nbsp;</p>

## FOR vs. while vs. DO while
---

1.  For: runs the program for a specific number of times;condition is usually a counter.



The for loop has the following syntax:

```json 
for (statement 1; statement 2; statement 3) {
  // code block to be executed
}
```

- Statement 1 is executed (one time) before the execution of the code block.

- Statement 2 defines the condition for executing the code block.

- Statement 3 is executed (every time) after the code block has been executed.
<p>&nbsp;</p>
<p>&nbsp;</p>
2. While: if you don't know how many times you should run a program; you can use other than the counter.

``` json
while (condition) {
  // code block to be executed
}
```
<p>&nbsp;</p>
<p>&nbsp;</p>

 3. Do while: similar to while but will run the code block at least one time even if the condition started as false.




