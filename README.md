RebeliX X3
=======
RebeliX X3 - a 3D printer based on MLAB's variant of RbeliX open-source 3D printer. New version will be constructed with [igus bearings](https://www.igus.cz/drylin/linear-guide). We are using [this](https://github.com/nophead/NopSCADlib) OpenSCAD library.

Features
=====

* Piezoelectric based precise Z-calibration
* Symmetric motor configuration push-pull to minimize belt stretching in printing of corners



![RebeliX](Rebelix_render.png "Preview of assembled printer" )



Build
=====

   sudo pip install stlsort


To continue OpenSCAD has to be installed and available as `openscad` command.

1. Make necessary changes to configuration.scad according to printer that prints the parts and available hardware. 
* Generate a calibration object by `make calibration`.
* Print generated calibration.stl and repeat the steps if unhappy.

When satisfied, run `make clean && make all`. That produces STLs with your tweeks.

