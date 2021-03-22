<p>&nbsp;</p>

# Readings : CSS Layout

## What's the difference between **Block-level** & ** Inline** elements ?

- Block-level elements start on a new line Examples include:
`<h1> <p> <ul> <li>`

- Inline elements flow in between surrounding text Examples include:
`<img> <b> <i>`



<p>&nbsp;</p>
<p>&nbsp;</p>



> If one block sits inside another block then the the outer block is called the parent element.

<p>&nbsp;</p>

> when multiple elements sit together we usually use `<div>` to group them. 



<p>&nbsp;</p>
<p>&nbsp;</p>



## The position of elements can be :
1.  Normal flow:
     - static: An element with `position: static;` is not positioned in any special way; it is always positioned according to the normal flow of the page.
     
  <p>&nbsp;</p>
  <p>&nbsp;</p>

2.  Relative: An element with `position: relative;` is positioned relative to its normal position.
   > Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position. Other content will not be adjusted to fit into any gap left by the element.

<p>&nbsp;</p>
<p>&nbsp;</p>

3.  Absolute: An element with `position: absolute;` is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).
> However; if an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.

<p>&nbsp;</p>
<p>&nbsp;</p>

4. An element with `position: sticky;` is positioned based on the user's scroll position.

> A sticky element toggles between relative and fixed, depending on the scroll position. It is positioned relative until a given offset position is met in the viewport - then it "sticks" in place (like position:fixed).

> You must specify at least one of `top`, `right`, `bottom` or left for sticky positioning to work.

<p>&nbsp;</p>
<p>&nbsp;</p>

5. fixed
<p>&nbsp;</p>
<p>&nbsp;</p>

6.  overlapping elements : use the z-index.; When elements are positioned, they can overlap other elements.
> The z-index property specifies the stack order of an element (which element should be placed in front of, or behind, the others).
>An element can have a positive or negative stack order.

`z-index: -1;`   means that this element will be in the background of the overlapping element.

<p>&nbsp;</p>
<p>&nbsp;</p>

---


## Some factors you need to take in consideration when designing the layout of your web page:

- Screen sizes effects.
- Screen Resolutions effects.
- page sizes.



<p>&nbsp;</p>
<p>&nbsp;</p>

## Type of layouts:
- Fixed layout: it doesn't change size no matter what the size of the browser window was.
- Liquid layout: the design changes to fit the screen.


<p>&nbsp;</p>
<p>&nbsp;</p>


<p>&nbsp;</p>
<p>&nbsp;</p>


<p>&nbsp;</p>
<p>&nbsp;</p>







# References 
1. From the Duckett HTML book:
   - HTML/CSS book, Ch. 15, “Layout”.