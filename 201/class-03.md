Readings : HTML Lists, Control Flow with JS, and the CSS Box Model
## LISTS
---

### there are three main types of lists used in HTML:
1. unordered lists: where each item in the list  starts with a bullet.

```html
<ul>
<li> item 1 </li>
<li> item 2 </li >
.....
</ul>
````
<p>&nbsp;</p>


2. ordered lists: where each item in the list starts with a number(or a numbering system).

```html
<ol>
<li> item 1 </li>
<li> item 2 </li >
.....
</ol>
````
<p>&nbsp;</p>


3. definition lists: where we list items and define them


```html
<dl>
<dt> the term </dt>
<dd> the definition </dd>
</dl>
```

## what are nested lists?
- They are lists within lists; so you may have a list then one item will have options or multiple types and you list them in a sub-list.


## BOXES
---

Each element in an HTML page will be in a box; it is important to control how these boxes appear.

 ### some properties that control the boxes:

1. box dimensions: In order to define your box you should define its height and its width in your CSS file. <p>&nbsp;</p>
 

```css
div{
    height= 75%;
    width=75%;
}
```

<p>&nbsp;</p>


### how to define the value inside the height and width attributes ?
1. percentage: where the box will be defined relative to the screen. 

2. using ems: where the size of th box is defined relative to the text within.

3. px: where the size is defined by pixels.


> The percentage is how most web pages are defined, but recently developers and designers began using px and ems to make the web page compatible with different devices and browsers.



### legibility (clear enough to read)
This is an important quality to have when designing a web page. 
why is legibility important?

- Some page designs expand and
shrink to fit the size of the user's
screen.


-  the min-width property specifies
the smallest size a box can be
displayed at when the browser
window is narrow.

- max-width property indicates
the maximum width a box can
stretch to when the browser
window is wide.
<p>&nbsp;</p>
<p>&nbsp;</p>



> we use the max-width property to make sure the lines are not very wide in a full-size browser window.
> we use the min-width property to make sure they don't appear very narrow.

<p>&nbsp;</p>
<p>&nbsp;</p>



### Overflow content:
The overflow property is used to tell the
browser what to do when the content inside a box is bigger than the box contained in it. 
<p>&nbsp;</p>


It can have one of these two values:
- hidden: where extra content that doesn't fit gets hidden.

- scroll:where a scrollbar is added to the box and the user can scroll to see the content not shown due to being larger than the box it is in.
<p>&nbsp;</p>


### borders, margins, paddings
--- 

### what's the difference between theses three concepts?
1. borders; each box has its borders even if it's width was set to zero pixels.

2. margins: theses are used to create gaps between boxes.

3. paddings: these specify the space between the border of the box and its content.
<p>&nbsp;</p>

> note: When you define the width of a box the border, margin and padding will be added to that value.

<p>&nbsp;</p>


### What is an Array?
An array is like a variable but can hold more than one value inside it.

<p>&nbsp;</p>

What is the syntax of Arrays?

`var name = [item1, item2, item3];`

    
<p>&nbsp;</p> 

How to access an Array element?
the first element will be given an index number **zero** and the second will be one and so on.
- so to call an element use:

`Array_name[index_number];`
- you can assign this element to a variable:

`var element= Array[1];` ..... this will assign the value of the second element in the array to the variable element.


<p>&nbsp;</p>

## LOOPS AND DECISIONS:
---

### Why do we use loops ?
- We use loops to create and control the flow of data in our scripts in order to handle different situations.


### there are three main types of loops:
1. While
2. DO - while
3. for loop


<p>&nbsp;</p>
<p>&nbsp;</p>

# why do we use SWITCH?
the switch starts with the variable inside the `( )`  it is called the switch variable, then we state different cases with statement that will run when the case actualizes.

<p>&nbsp;</p>

> Each case will not end and will run the next case unless you made sure you add the `break;` after it.
 
 <p>&nbsp;</p>


> if no case applies then a default case must be defined and it will run automatically.
<p>&nbsp;</p>


```
switch(var){
    case 'value' : 
    statement
    break;
     case 'another value':
     statement
     break;
     default 'default case':
     statement
     break;
         }
```







References:
-----
1. From the Duckett HTML book:
    - Chapter 3: “Lists” (pp.62-73)
    - Chapter 13: “Boxes” (pp.300-329)


2. From the Duckett JS book:
    - Chapter 2: “Basic JavaScript Instructions” (pp.70-73)
    - Chapter 4: “Decisions and Loops” from switch statements on (pp.162-182)