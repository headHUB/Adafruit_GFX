This is a variation of the Adafruit_GFX library. It has been modified to don't broken compatibility with regular one
but since the text method it's changed and it's experimental (now it's faster and support multiple fonts) YOU CAN FIND SOME SMALL PROBLEMS WHEN DISPLAY TEXT.
The modifications:
 - Faster Circle rendering
 - Faster Font Rendering
 - Multiple font support
 - Expanded bitmap support
 - Added ellipse rendering (with fast sin e cos tables)
 
If uou are using a library that include this one you will probably get an error during compilation about <b>glcdfont</b>!!!
Solution it's simple, if you want to use this library you just comment out the include of glcdfont in the library that uses
this verion of Adafruit_GFX as:<br>

//#include "glcdfont.c" //comment out if you are using the custom version of Adafruit_GFX!!!!!!!!!

That's it.


This is the core graphics library for all our displays, providing a common set of graphics primitives (points, lines, circles, etc.).  It needs to be paired with a hardware-specific library for each display device we carry (to handle the lower-level functions).

Adafruit invests time and resources providing this open source code, please support Adafruit and open-source hardware by purchasing products from Adafruit!

Written by Limor Fried/Ladyada for Adafruit Industries.
BSD license, check license.txt for more information.
All text above must be included in any redistribution.

To download, click the DOWNLOAD ZIP button, uncompress and rename the uncompressed folder Adafruit_GFX. Confirm that the Adafruit_GFX folder contains Adafruit_GFX.cpp and Adafruit_GFX.h

Place the Adafruit_GFX library folder your <arduinosketchfolder>/Libraries/ folder. You may need to create the Libraries subfolder if its your first library. Restart the IDE.
