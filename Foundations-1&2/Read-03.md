## Responsive Web Design
* what is it:
    * the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop
    * focused around providing an intuitive and gratifying experience for everyone
 * responsive vs. adaptive vs. mobile
    * responsive and adaptive web design are closely related, and often transposed as one in the same
    * mobile, on the other hand, generally means to build a separate website commonly on a new domain solely for mobile users
    * currently the most popular technique lies within responsive web design, favoring design that dynamically adapts to different browser and device viewports, changing layout and content along the way

## All About Floats
* Example: 
```
#sidebar {
  float: right;			
}
```
* left, right, none, inherit (which assumes the float value of the parent)
* clearing the float:
    * an element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float
* problems with float:
    * pushdown: when an element inside a floated item being wider than the float itself (typically an image)
    * quick fix = overflow:hidden
* reference: CSS Floats Explained by Riding an Escalator 
