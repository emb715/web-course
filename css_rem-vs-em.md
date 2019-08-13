# REM vs EM
Why REM OR EM and not px? When using rem or em the values are flexible, they are relative units, it depends on the font-size, is a multiplier.

Ex: by default browser have a 16px font size.
~~~
html { font-size: 16px; }
div { font-size: 1rem; }
p { font-size: 1em; }
~~~~

The ```div``` and ```p``` tags have a font-size of 16px, ```16px * 1 = 16px```, if we change the default value it will change our relative units.

~~~
html {font-size: 100px;}
~~~

When we use rem or em is goinig to be ```100px * 1 = 100px``` or the amount of relatives units

~~~
html { font-size: 100px; }
div { font-size: 2rem; } // 200px
p { font-size: 4em; } // 400px
~~~

## Main Difference
The main difference between them is that **```em``` units scale of the font-size of the element**, it has inheritance, that may bring some troubles.
> EM: Equal to the computed value of the font-size property of the element on which it is used.

The **```rem``` unit scale of the font-size of the html**
> REM: Equal to the computed value of font-size on the root element.


Source: https://www.w3.org/TR/css3-values/#font-relative-lengths


---


More samples and an extended explanation. https://webdesign.tutsplus.com/tutorials/comprehensive-guide-when-to-use-em-vs-rem--cms-23984
