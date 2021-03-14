# ***Read: 02 - HTML Text, CSS Introduction, and Basic JavaScript Instructions***



# Basic Javascript Instructions
<p>&nbsp;</p>

- Each code line in JS is called a statement and should end with a semicolon `;` .
<p>&nbsp;</p>

- You can write a comment, which are descriptions or notes for developers, in two ways:
    - For a single line comment : type `//` and whatever is to the right of this will be a comment until the next line.
    - For multiple lines: use the following format:
    
    ```
    /*
    .....
    ...
    ..
    .
    */
    ``` 



    # What is a variable in JS?
    - A variable is a storage for bits where temporary data resides; it can change with each time the code is run.




    ### How do you declare a variable?
    - You can declare a variable using the following syntax:
    
     var name = value ;
    
  <p>&nbsp;</p>
  <p>&nbsp;</p>

    **Variable naming rules:**

    1. The name must start with a letter an (_) or a ($).
    2. the name can contain numbers, letters ,(_), ($).
    3. The name can **NOT** have a period or a score (-).
    4. You cannot use keywords (like var) or reserved words( that may be used in other versions).


    > *NOTE:*
    >1. variable name is case sensitive
    >2. You can use the camel technique when writing names that have two words or more like (CodeExpertIsHere).


<p>&nbsp;</p>

What is an Array?
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
Why do we use loops ?
- We use loops to create and control the flow of data in our scripts in order to handle different situations.

---
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>

> # **HTML Text**
---

### Texts:
- HTML has six levels of heading that range in size from h1 being the largest till h6.

![headings](https://qph.fs.quoracdn.net/main-qimg-a21e4d03936ffd09d6eb38db5749bc62)



- Any paragraph can be defined by using the tags:
```
<p>
 content text
</P>
```

### Styling the text content:
 - You can use the following tags to change the format of your font:
    - bold: `<b>`
    - italic: `<i>`
    - superscript:`<sup>` used in powers especially.

    - subscript: `<sub>` used in footnotes and chemical equations especially.

  <hr/>

<p>&nbsp;</p>


 -  How to add  a ***linebreak*** and a ***horizontal ruler***?

  `<br/>` is used to insert a line break; so the line ends and the next word will show on the next line.

  `<hr/>` this adds a horizontal ruler; helps with seperating content.

  <p>&nbsp;</p>
  <p>&nbsp;</p>


  ## STRONG Vs. EMPHASIS

  Strong is used to show that this content is important whereas emphasis is used to notify the reader that this will subtly change the meaning intended.
 
 ` <strong> it will get bold </strong>`

`<em> it will get italic </em>`


<hr/>

### **QUOTATION:**

1. Block quotes: used with long quotations 

```
<blockquote cite ="URL">
<P>
THE QUOTE
</P>
</blockquote>
```


2. short quotes: you can use the tag `<q> quote </q>`


<hr/>


## **CSS Instruction**

- In order to understand styling with CSS we need to think of each element as if it is in a box. This image will show how does it work.


![inside the box](/images/itb.png)


 <p>&nbsp;</p>
  <p>&nbsp;</p>

### How do we associate each element with a rule to style it?

1. First define your selector: which is basically the element you are trying to style.

2. open curly braces `{ }`

3. state an attribute and assign a value to it, ex. background-color:red;


>> note: you seperate between the attribute and the value by a colon and you must end each attribute with a semi colon.

 
<p>&nbsp;</p>
  <p>&nbsp;</p>

- There are different types of selectors such as; universal selectors (*), class selectors (.) as we mentioned in previous notes (check them!).

<p>&nbsp;</p>
  <p>&nbsp;</p>

###  WHY do we use external Style sheets? 
1. To avoid repeatition.
2. To make the script and code more clear.
3. To edit one file if the style is to be changed.
<p>&nbsp;</p>
  <p>&nbsp;</p>

### How CSS Rules Cascade?
1. latest if two selectors are 100% identical then the latest rule will apply[not chronologically but steps wise.]
2. specification: the more specified selector will get the attribute so if you use a class selector it will take precedence over a universal selector.




<p>&nbsp;</p>
  <p>&nbsp;</p>
<p>&nbsp;</p>
  <p>&nbsp;</p>
<p>&nbsp;</p>
  <p>&nbsp;</p>

---

References: 
1. From the Duckett HTML book:<br>
Chapter 2: “Text” (pp.40-61).<br>
Chapter 10: Ch.10 “Introducing CSS” (pp.226-245).<br>


 <p>&nbsp;</p>

2. From the Duckett JS book:<br>
Chapter 2: “Basic JavaScript Instructions” (pp.53-84)<br>
Chapter 4: “Decisions and Loops” only up to the section on switch statements (pp.145-162)<br>

3. The image showing the headings type is taken from this URL:(https://qph.fs.quoracdn.net/main-qimg-a21e4d03936ffd09d6eb38db5749bc62)