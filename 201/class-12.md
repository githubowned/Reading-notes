# Read: 12 - Docs for the HTML `<canvas>` Element & Chart.js

## Readings : Chart.js, Canvas
---
 Setting up

1. download Chart.js.
2. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. 
3. Then create a new html page and import the script.
<p>&nbsp;</p>
<p>&nbsp;</p>

```
<!DOCTYPE html>
<html lang="en">

    <head>

           <script src='Chart.min.js'></script>

    </head>

    <body>

    </body>

</html>
```
<p>&nbsp;</p>
<p>&nbsp;</p>

## The `<canvas>` element

- syntax:

`<canvas id="tutorial" width="150" height="150"></canvas>`


- width and height are OPTIONAL.
- When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high.

<p>&nbsp;</p>
<p>&nbsp;</p>

 ### To render Content; Use `.getContext('2d')`
```
var canvas = document.getElementById('tutorial');
var ctx = canvas.getContext('2d');

```
<p>&nbsp;</p>
<p>&nbsp;</p>

### The Grid:
- It's a coordinate space.
- Normally 1 unit in the grid corresponds to 1 pixel on the canvas. 
- The origin of this grid is positioned in the top left corner at coordinate (0,0).
-  All elements are placed relative to this origin.

<p>&nbsp;</p>
<p>&nbsp;</p>


### Drawing rectangles

1. fillRect(x, y, width, height)
- Draws a filled rectangle.
2. strokeRect(x, y, width, height)
- Draws a rectangular outline.
3. clearRect(x, y, width, height)
- Clears the specified rectangular area, making it fully transparent.


<p>&nbsp;</p>
<p>&nbsp;</p>

### Drawing paths
1. you create the path.
2. you use drawing commands to draw into the path.
3. you can stroke or fill the path to render it.

<p>&nbsp;</p>
<p>&nbsp;</p>


1. beginPath()
- Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
Path methods
Methods to set different paths for objects.
2. closePath()
- Adds a straight line to the path, going to the start of the current sub-path.
3. stroke()
- Draws the shape by stroking its outline.
4. fill()
Draws a solid shape by filling the path's content area.

<p>&nbsp;</p>
<p>&nbsp;</p>


 ##  How to create a bar chart for a single dataset and render that ?

```
 <canvas id="myChart" width="400" height="400"></canvas>
<script>
var ctx = document.getElementById('myChart').getContext('2d');
var myChart = new Chart(ctx, {
    type: 'bar',
    data: {
        labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],
        datasets: [{
            label: '# of Votes',
            data: [12, 19, 3, 5, 2, 3],
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)',
                'rgba(54, 162, 235, 0.2)',
                'rgba(255, 206, 86, 0.2)',
                'rgba(75, 192, 192, 0.2)',
                'rgba(153, 102, 255, 0.2)',
                'rgba(255, 159, 64, 0.2)'
            ],
            borderColor: [
                'rgba(255, 99, 132, 1)',
                'rgba(54, 162, 235, 1)',
                'rgba(255, 206, 86, 1)',
                'rgba(75, 192, 192, 1)',
                'rgba(153, 102, 255, 1)',
                'rgba(255, 159, 64, 1)'
            ],
            borderWidth: 1
        }]
    },
    options: {
        scales: {
            yAxes: [{
                ticks: {
                    beginAtZero: true
                }
            }]
        }
    }
});
</script>
```
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>


# References:
1. https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/

2. https://www.chartjs.org/docs/latest/

3. https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage

