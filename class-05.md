## HTML, Chap 5, pg 94 - 125
* storing images inside of your project folder is probs the best route, also cleaner, also no gigantic links
* < img src = "link" followed by alt = "description of img" > is best practice for accessibility purposes 
* height and width can also be done inside the img tag itself 
* align = "left or right" relative to < p > tags tell the img where to sit next to text
* same as above, but vertical, is align = "top, bottom, middle"
* img are best when jpeg, gif, or png - saving with incorrect format could result in img dysfunction
    * jpeg = colorful pics with heavy resolution
    * gif/png = few colors or large areas of the same color
* yo pixels? tiny squares.
* vector images = logos
* < figure < img src = > < figcaption> > captions your img

## HTML, Chap 11, pg 246 - 263
* color:
* background-color:
* opacity: 0.5
    * 0.5 = 50% (opacity)
    * some older browser can't do opacity, rgba colors
    * you can offer a fallback (not sure how, tho, even after reading this part)
* HSLA = hue, saturation, lightness, alpha
    * hue expressed an angle between 0 and 360
    * saturation " as a percentage
    * lightness is 0% = white, 50% = normal, 100% = black
    * alpha, basically transparency, " as decimal btw 0 and 1; 0.5 = 50% transp for example

## HTML, Chap 12, pg 264 - 299
* typeface
    * serif = extra details on the letter ends
    * sans serif = straight letter ends
    * monospace = every letter is fixed width 
    * weight = boldness
    * style = italics
    * stretch = condensed or extended 
* know that a typeface will only display if its in the computer 
    * OR if you use @fontface and import url or saved file in your code
* text-transform
    * uppercase, lowercase, capitalize
* text-decoration
    * underline, overline, line through, blink (annoying, don't do it)
* ps. em is the width of an m -- what. a. metric
* line-height
    * equivalent to the leading, aka the space above the text
* letter/word spacing
    * kerning = space between each letter
    * uses ems, everything pretty much uses ems
* text-align
    * left, right, center, justify
* vertical-align
    * baseline, sub, super, top, text-top, middle, bottom, text-bottom
* text-indent
    * use px
    * indents the first line of text within an element
* text-shadow
    * takes up to 3 length, in px, and a color for the shadow
    * i like #111111
* id : first letter, : first line
    * makes the fist letter in the first line in whatever text section look storybook bold and fancy
* : link and : visited
    * changes the color of your link once you've clicked it
* : hover, : active, : focus
    * hover changes color of whatever you hover over
    * active changes the color of whatever you click and make active
    * focus is "applied when an element has focus" (??? um, ok.)

