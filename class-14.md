## CSS Transforms
* 2D/3D tranforms:
    * transform accepts a handful of diff values 
        * rotate = uses 0 - 360 degrees
        * default point of rotation 50% 50%
* 2D/3D scale
    * scale value goes inside transform property
        * default scale value is 1 
        * therefore btw .01 and .99 makes an element appear smaller
        * value over 1, appears bigger
* 2D/3D translate
    * works like relative positioning, pushing and pulling an element
    * translateY
    * translateX
* 2D/3D skew
    * distorts elements on the H and V axis (x, y)
    * measured in units of degrees
    * no pixels or percentages

## CSS Transitions & Animations
 * easiest ways of determining styles for diff states
    * :hover
    * :focus
    * :active
    * :target
* for transition related properties
    * transition-property = color, font size, etc. (display)
    * transition-duration = duration in which a transition takes place
    * transition-timing-function = sets the speed in which the transition will move
    * transition-delay = determines how long a transition should be stalled before executing
* refer to this article for transitional properties
    * the list is too long to type in here, correspond to transition-property above
    * https://learn.shayhowe.com/advanced-html-css/transitions-animations/
   
## CSS3 transitions
* fade in 
    * coded in two steps: first, you set the initial state; next, you set the change
* change color
    * we just set the div’s class to “color” and specify the color we want in our CSS
* grow & shrink
    * give your div the class "grow" (and "shrink"? doesn't specify)
    ```
    .grow:hover
    {
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
    }
    .shrink:hover
    {
        -webkit-transform: scale(0.8);
        -ms-transform: scale(0.8);
        transform: scale(0.8);
    }
    ```
* rotate elements
    * give your div the class "rotate"
    ```
    .rotate:hover
    {
        -webkit-transform: rotateZ(-30deg);
        -ms-transform: rotateZ(-30deg);
        transform: rotateZ(-30deg);
    }
    ```
* square to circle
    * give your div the class "circle"
    ```
    .circle:hover
    {
        border-radius:50%;
    }   
    ```
* 3D shadow
    * give your div the class "threed"
    ```
    .threed:hover
    {
        box-shadow:
                1px 1px #53a7ea,
                2px 2px #53a7ea,
                3px 3px #53a7ea;
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
    }
    ```
* swing
    * reference articles, too much code to cut and paste 

* inset border
    * give your div the class "border"
    ```
    .border:hover
    {
        box-shadow: inset 0 0 0 25px #53a7ea;
    }
    ```
## 6 Buttons animated
* great example code for animated buttons 
    * https://codepen.io/retyui/pen/ByoaXV

## CSS3 Animations: Keyframes
* for future reference, more example code on keyframe animation:
    * https://codepen.io/akshaychauhan/pen/oAfae

## 404
* WHOOOOAAAA 404 MAAAAN TRIPPYYYY
    * future ref: https://codepen.io/kieranfivestars/pen/MYdQxX

## Pure CSS Bounce Animation
* example of importing @keyframe use in animation, plus good animation example code 
    * future ref: https://codepen.io/dp_lewis/pen/gCfBv
