Read: 05 - HTML Images; CSS Color & Text

# Images
-  When picking an image for your website; that image should be relevant and would convey a specific message.

<p>&nbsp;</p>

### The <img> tag has two required attributes:

- src - Specifies the path to the image.
- alt - Specifies an alternate text for the image.

<p>&nbsp;</p>

### We use the following Syntax
 
`<img src="url" alt="alternatetext">`

<p>&nbsp;</p>

> If a browser cannot find an image, it will display the value of the alt attribute.

<p>&nbsp;</p>
<p>&nbsp;</p>

## JPEG Vs. PNG Vs. Gif:

- We Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth.

- We Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos.

- We Use GIF format for images that contain animations.

<p>&nbsp;</p>
<p>&nbsp;</p>

# Colors 

Color codes are ways of representing the colors we see everyday in a format that a computer can interpret and display. Commonly used in websites and other software applications, there are a variety of formats, including Hex color codes, RGB and HSL values, and HTML color names, amongst others.


- Hexadecimal colors
- RGB colors
- RGBA colors
- HSL colors
- HSLA colors



![GIF COLOR WHEEL](https://99designs-blog.imgix.net/blog/wp-content/uploads/2017/02/Color-Wheel-2.gif?auto=format&q=60&fit=max&w=930)


<p>&nbsp;</p>
<p>&nbsp;</p>


# Text

The properties that allow you to control the appearance of text are so many and so different.


### CSS Text Shadow
The CSS text-shadow property applies shadow to text.


<p>&nbsp;</p>

- Syntax of text shadow:
```
h1 {
  text-shadow: 2px 2px;
}
```


<p>&nbsp;</p>

<p>&nbsp;</p>

### Text Color and Background Color
In this example, the background-color property and the color property are both defined:


<p>&nbsp;</p>

```
body {
  background-color: lightgrey;
  color: blue;
}

h1 {
  background-color: black;
  color: white;
}
```


### Text Alignment
-The text-align property is used to set the horizontal alignment of a text.

- A text can be :
1. left.
2. right.
3. centered.
4. justified.


```
h1 {
  text-align: center;
}
```






<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>












# References:

- From the Duckett HTML book:
   - Chapter 5: “Images” (pp.94-125).
   - Chapter 11: “Color” (pp.246-263).
   - Chapter 12: “Text” (pp.264-299).