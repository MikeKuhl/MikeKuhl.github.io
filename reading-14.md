# Advanced CSS #

- The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

 - The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

 ```div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
} ```



 - Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis.

 - The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Positive is clockwise/Negative is counterclockwise.

- Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1. .99 and .01 makes an element appear smaller for example.

- The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document. Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.
