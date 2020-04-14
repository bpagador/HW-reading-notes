## Easily Create Stunning Animated Charts with Chart.js
* charts are better than tables, ya heard 
* refer to this document for guided chart examples 

## Chart.js docs
* refer this to download chart.js into your GitHub

## Basic usage
* < canvas > elemeny only has 2 values
    * width and height 
    * when these attibutes are not specified, the default is 300px wide, 150px high
    * can be sized by CSS
* always a good idea to provide id to the html element 
* canvas element can be styled like any normal image 
* these rules don't affect the actual drawing 
* fallback content is recommended either in text or sub DOM
* canvas element requires a closing tag 
* getContext() = tells canvas what type of display to render 
    * remember to first retrieve the element in the DOM using getElementById
* you can attach a conditional statement to getContext to tell the scrip to check for browser support 
* SKELETON TEMPLATE provided, refer back to this API

## Drawing shapes with canvas
* the grid:
    * normally, 1 unit in the grid corresponds to 1 pixel on the canvas 
    * the origin of this grid is positioned in the top left corner at coordinate (0,0)
* drawing rectangles:
    * fillRect (x, y, width, height) = draws a filled rect
    * strokeRect (x, y, width, height) = draws an outline
    * clearRect (x, y, width, height) = clears the specified rect area, makes it transparent
* drawing paths:
    * a list of points, connected by segments of lines that can be shaped, colored in however
    * to make shapes using paths:
        1. create path
        2. use drawing commands to draw into the path
        3. once path is creayed, stroke or fill path to render it 
    * drawing commands:
        * beginPath() = creates a new path
        * closePath() = adds a straight line to the path, going to the start of the current sub-path
        * stroke() = draws shape by stroking its outline
        * fill() = draws a shape by filling te path's content area
## Applying styles and colors
* apply colors to a shape
    * fillStyle = color
        * sets the style used when filling shapes.
    * strokeStyle = color
        * sets the style for shapes' outlines.
* we can also draw semi-transparent (or translucent) shapes
    * globalAlpha = transparencyValue
        * applies the specified transparency value to all future shapes drawn on the canvas. 
        * the value must be between 0.0 (fully transparent) to 1.0 (fully opaque). 
        * this value is 1.0 (fully opaque) by default.
* line styles 
    * lineWidth = value
        * sets the width of lines drawn in the future.
    * lineCap = type
        * sets the appearance of the ends of lines.
    * lineJoin = type
        * sets the appearance of the "corners" where lines meet.
    * miterLimit = value
        * establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
    * getLineDash()
        * returns the current line dash pattern array containing an even number of non-negative numbers.
    * setLineDash(segments)
        * sets the current line dash pattern.
    * lineDashOffset = value
        * specifies where to start a dash array on a line.
## Drawing text
* fillText(text, x, y [, maxWidth])
    * fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
* strokeText(text, x, y [, maxWidth])
    * strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.