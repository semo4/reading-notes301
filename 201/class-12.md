# Class 12 Reading

# Chart.js, Canvas

## EASILY CREATE STUNNING ANIMATED CHARTS WITH CHART.JS
- Chart are not easy to create but it is better to display data and explain it 
- there are many type of charts:
    1. bar charts
    2. line charts
    3. pie charts

- we can use chart in javascript it is plugin in javascript and in html it can be used by  `<canvas>` element

## Drawing a line chart
- if we want to draw line we have to write in html  `<canvas>` element
- then we go and idintify the canvas in javascript to display the data inside the chart that we create 


## Drawing a pie chart
- we will use same step to create a pie chart but the deferent is the data we will use 

## Drawing a bar chart
- it we be create the chart like the line chart.

# Conclusion
- The great things about Chart.js are that it’s simple to use and really very flexible.

# Canvas API.
## Basic usage of canvas
### The `<canvas>` element
- we can use canvas like img tag 
- canvase take two value width an height 
- ` <canvas id="tutorial" width="150" height="150"></canvas>` 


### Fallback content
- Providing fallback content is very straightforward
- we can do it by insert contect inside the canvas 
- some browsers does'n support canvas we must provide feedback

### The rendering context
- we can use context with canvas 
- it can take two value 2d and 3d

### Checking for support
- there is some browsers do not support `<canvas>` 

### A skeleton template
- The script includes a function called draw(), which is executed once the page finishes loading


# Drawing shapes with canvas
## The grid
- if we want to draw grid ther is consept in canvas  known as
grid or coordinate space

## Drawing rectangles
-  ` <canvas>`  only supports two primitive shapes: rectangles and paths (lists of points connected by lines)
- All other shapes must be created by combining one or more paths
- There are three functions that draw rectangles on the canvas:
1. fillRect(x, y, width, height)
    - Draws a filled rectangle.
2. strokeRect(x, y, width, height)
    - Draws a rectangular outline.
3. clearRect(x, y, width, height)
    - Clears the specified rectangular area, making it fully transparent.

## Drawing paths
- path is set of point 
- connected by segments of lines that can be of different shapes
- curved or not
- different width and of different color
-  can be closed
- Here are the functions used to perform these steps:
1. beginPath()
    Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
    Path methods
    Methods to set different paths for objects.
2. closePath()
    Adds a straight line to the path, going to the start of the current sub-path.
3. stroke()
    Draws the shape by stroking its outline.
4. fill()
    Draws a solid shape by filling the path's content area.

## Moving the pen
- which doesn't actually draw anything but becomes part of the path
- moveTo(x, y)
    - Moves the pen to the coordinates specified by x and y.

## Lines
- For drawing straight lines, use the lineTo() method.

- lineTo(x, y)
    - Draws a line from the current drawing position to the position specified by x and y.

## Arcs
- To draw arcs or circles, we use the arc() or arcTo() methods.

- arc(x, y, radius, startAngle, endAngle, anticlockwise)
    - Draws an arc which is centered at (x, y) position with radius r starting at startAngle and ending at endAngle going in the given direction indicated by anticlockwise (defaulting to clockwise).
- arcTo(x1, y1, x2, y2, radius)
    - Draws an arc with the given control points and radius, connected to the previous point by a straight line.


## Bezier and quadratic curves
- The next type of paths available are Bézier curves, available in both cubic and quadratic varieties. These are generally used to draw complex organic shapes.

- quadraticCurveTo(cp1x, cp1y, x, y)
    - Draws a quadratic Bézier curve from the current pen position to the end point specified by x and y, using the control point specified by cp1x and cp1y.
- bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)
    - Draws a cubic Bézier curve from the current pen position to the end point specified by x and y, using the control points specified by (cp1x, cp1y) and (cp2x, cp2y).

## Rectangles
- In addition to the three methods we saw in Drawing rectangles, which draw rectangular shapes directly to the canvas, there's also the rect() method, which adds a rectangular path to a currently open path.

- rect(x, y, width, height)
    - Draws a rectangle whose top-left corner is specified by (x, y) with the specified width and height.


# Applying styles and colors
## Colors
- we can add color to shap by two ways:
1. fillStyle = color
    - Sets the style used when filling shapes.
2. strokeStyle = color
    - Sets the style for shapes' outlines.

## Line styles
- There are several properties which allow us to style lines.

- lineWidth = value
    -Sets the width of lines drawn in the future.
- lineCap = type
    - Sets the appearance of the ends of lines.
- lineJoin = type
    - Sets the appearance of the "corners" where lines meet.
- miterLimit = value
    - Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
- getLineDash()
    - Returns the current line dash pattern array containing an even number of non-negative numbers.
- setLineDash(segments)
    - Sets the current line dash pattern.
- lineDashOffset = value
    - Specifies where to start a dash array on a line.

## Gradients
- we can fill and stroke shapes using linear and radial gradients
- there are two value: 
- createLinearGradient(x1, y1, x2, y2)
    - Creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2).
- createRadialGradient(x1, y1, r1, x2, y2, r2)
    - Creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1) and a radius of r1, and the other with its center at (x2, y2) with a radius of r2.

## Patterns
- we used a series of loops to create a pattern of images
- we use this method to create pattren and it take two parameters:
- createPattern(image, type)
- type it take multiple value :
    - repeat
        - Tiles the image in both vertical and horizontal directions.
    - repeat-x
        - Tiles the image horizontally but not vertically.
    - repeat-y
        - Tiles the image vertically but not horizontally.
    - no-repeat
        - Doesn't tile the image. It's used only once.

## Shadows
- Using shadows involves just four properties:

- shadowOffsetX = float
    - Indicates the horizontal distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
- shadowOffsetY = float
    - Indicates the vertical distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
- shadowBlur = float
    - Indicates the size of the blurring effect; this value doesn't correspond to a number of pixels and is not affected by the current transformation matrix. The default value is 0.
- shadowColor = color
    - A standard CSS color value indicating the color of the shadow effect; by default, it is fully-transparent black.


# Drawing text
## Drawing text
- The canvas rendering context provides two methods to render text:

- fillText(text, x, y [, maxWidth])
    - Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
- strokeText(text, x, y [, maxWidth])
    - Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

## Styling text
- There are some more properties which let you adjust the way the text gets displayed on the canvas:

- font = value
    - The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
- textAlign = value
    - Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
- textBaseline = value
    - Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
- direction = value
    - Directionality. Possible values: ltr, rtl, inherit. The default value is inherit

## Advanced text measurements
- In the case you need to obtain more details about the text, the following method allows you to measure it.

- measureText()
    - Returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn in the current text style.
