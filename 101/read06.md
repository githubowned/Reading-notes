# READ:O6b - Design webpages with CSS
---

## **what is CSS ?**
It is short for cascading style sheets.
why do we use it ? we use it to change the styling an layout of our web pages.
<p>&nbsp;</p>

### How do we use it ?
- Inline : it is included in the same tag in the HTML file.

- External: it is saved on a seperate file with the extension `.css `.

- Internal: within the same HTML file but will not be included within the body of the webpage; rather it will be included in the head part of the webpage.
<p>&nbsp;</p>

<p>&nbsp;</p>

### How the inline method works?<br>

`<p style="color:red;"> `

<p>&nbsp;</p>


### How the internal method work?<br>

``` <head>
<style>
p{color: red ;}
</style> 
</head>
```
### How the external method work?<br>
```
<head>
<link rel="stylesheet" href"styles.css" >
</head>
```

## Colors:

There are many ways of choosing colours to add on your elements:
1. name of the colour `{ color:blue ;}`
2. hex (## -- -- --)
3. rgb()
4. hsl


RGB Values
---
Values for red, green, and blue
are expressed as numbers
between 0 and 255.

Hex Codes
---
Hex values represent values
for red, green, and blue in
hexadecimal code.

<p>&nbsp;</p>
<p>&nbsp;</p>

> HSL is short for hue, saturation and lightness

<p>&nbsp;</p>
Hue
---
Hue is near to the colloquial idea
of color. Technically speaking
however, a color can also have
saturation and brightness as
well as hue.
<p>&nbsp;</p>
Saturation
---
Saturation refers to the amount
of gray in a color. At maximum
saturation, there would be no
gray in the color. At minimum
saturation, the color would be
mostly gray.
<p>&nbsp;</p>
Brightness
---
Brightness (or "value") refers
to how much black is in a color.
At maximum brightness, there
would be no black in the color.
At minimum brightness, the
<p>&nbsp;</p>


### **What does the "a" stand for in rgba or hsla?**
introduces the opacity
property which allows you to
specify the opacity of an element
and any of its child elements.
The value is a number between
0.0 and 1.0 (so a value of 0.5
is 50% opacity and 0.15 is 15%
opacity).


