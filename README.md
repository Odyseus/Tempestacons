[![icon-num](https://img.shields.io/badge/icons-116-blue.svg?style=flat-square)](#)
[![ License ](https://img.shields.io/badge/license-CC--BY--SA--4.0--intl-brightgreen.svg?style=flat-square)](LICENSE)

##Tempestacons

A set of 120 weather based svg icons.

![preview](preview.png)

###Rendering png's

The `render-pngs.sh` script will render png's from the `icons.svg` file by looping over the content of the `index.txt` file. Only id's inside the `index.txt` file will  be rendered.

* The script requires [Inkscape](https://inkscape.org/en/).

* The script doesn't overwrite files. Delete the file you want to ovewrite before executing the script.

* If you change the icon color swatch in the `icons.svg` file, update the `DEFULT_COLOR` variable inside the `render-pngs.sh` script, otherwise the script won't be able to change the png color during rendering. 

###Pseudo-artboards

Since inkscape doesn't have artboards, the `icon.svg` file provides pseudo-artboard support by grouping each icon with a rectangle, which represents the icon's canvas (32x32 in this set.)

The groups are given id's which represent the name of the exported png.

**NOTE** Color swatches are provided in the `icons.svg` file for easily changing the icon and grid colors as well as for hiding the icon-canvas rectangles before exporting.