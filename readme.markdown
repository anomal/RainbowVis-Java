RainbowVis-Java
=============

A Java library for (HTML/CSS) colour data visualization. Easily map numbers to a smooth-transitioning colour legend.

The Rainbow class by default maps the range 0 to 100 (inclusive) to the colours of the rainbow (i.e., a gradient transitioning from red to yellow to lime to blue).

`Rainbow rainbow = new Rainbow();` creates new instance of Rainbow. By default, the number range is from 0 to 100, and the spectrum is a rainbow.

`rainbow.colourAt(number)` returns the hex colour corresponding to the number as a String. If number is out of range, it returns the appropriate hex colour String corresponding to either the minNumber or maxNumber.

`rainbow.setSpectrum(colour1, colour2 [,colourN]);` sets the spectrum of the Rainbow object. By default, the spectrum is a rainbow. You must have a minimum of two colours, but you can specify more than two colours. Colours can be in the form "red", "ff0000", or "#ff0000". For example, `rainbow.setSpectrum("red", "yellow", "white");` makes the "Rainbow" a colour gradient from red to yellow to white.  

`rainbow.setNumberRange(minNumber, maxNumber);` sets the number range of the Rainbow object. By default, it is 0 to 100.

See the javadoc for more details.

Related Libraries
-----------------

* [RainbowVis-JS](https://github.com/anomal/RainbowVis-JS) - JavaScript version
