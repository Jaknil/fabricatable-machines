
A *fabricatable machine* is a computer-controlled fabrication machine that can be made using a standard set of existing computer-controlled machines; with minimal use of speciality parts, processes or skills.
The type of machines include CNC-milling, lasercutter, and 3d-printers.

We want to enable individuals and communities to build their own production machines, to expand their own capabilities.
Build more machines to increase production, build cheaper to increase availability, or build specialized machines tailored for specific purposes.


# Chamfer Rail

A linear actuator with rack & pinion drive system, designed to be CNC-milled.
This is a simplified version of the axis system from [V-bird](#V-bird) and [Simple Gantry](#simple-gantry),
which can be reproduced using only standard CNC operations and bits (chamfering using a 90deg V-bit). 

Additionally the pitch is slightly smaller, for higher resolution and torque.

The files included here are for NEMA17 sized motor.

[FreeCAD source](./chamferrail/chamferrail.fcstd)

# Award Plotter

* Pen plotter.
* Servo-based Z-axis

## TODO: Document



## [TapeXY](https://github.com/jonnor/tapecore/tree/master/README.md#tapexy)

A CoreXY-based motion platform using low-friction tape for plain bearings.
Designed for low-force end-effectors, easy reproduction using lasercutter + FDM 3d-printer.


# V-bird

* Presented during the [FAB12 conference](http://fab12.fabevent.org/).
* Standardized axis
* Assembled together into a CNC-mill


## TODO: Document


# Simple Gantry

Our first complete XY platform designed to be fabricated in a Fablab.
It can be used to build custom digital fabrication machines, from laserengraving to light-duty milling.
Initial prototype is for a gantry-based vinyl/laser-cutter. Video from fabricating the first gantry rig [here](https://youtu.be/k9ujdUikcWI)

![Laserengraving using diode-laser](./simple-gantry/img/laserengraving.jpg)

![First gantry prototype fabricated on Shopbot](./simple-gantry/img/simple%20gantry%20640%20x%20320%20test.JPG)

![First prototype linear axis fabricated on Shopbot](./simple-gantry/img/simplegantry-firstaxis.jpg)

![Machine builder interface](./simple-gantry/img/machine%20builder%20interface%20-%20simple%20gantry%20640%20x%20320.png)

## Status

**No longer developed**

## Core principles

* Using a birdbeak bit to make V-profiles, both inner and outer.
* Using technical low-friction plastics (UHWMPE/POM) motion/contact parts
* Assembling and contining to machine the axes on the CNC itself


## Tests

Laserengraving

![Laserengraving in plywood](./simple-gantry/img/laserengraving-helloworld.jpg)

* 10mm/s workspeed, 20 mm/s jog, 0.9 Amps laser power.
* Gcode generated by Cura, from a STL.
* No software control of the laserdiode (manually turned on off)
* Some of the bad lines are actually due to the poor quality font rendering
* At this speed will also (generally) cut through standard white printer paper


# Milestones

* Make an axis that is longer than the workarea.
Either by moving the workpiece, or machine in stages.
* A machine has been reproduced independently by someone else
* Use the machine in for realizing a project
* Have a machine that can fully reproduce itself

# Ideas

* Fabricate V-wheel for standard bearing using Shopbot with birdbeak/birdmouth bit

# Resources

Open source lasercutting software

* http://www.shapeoko.com/wiki/index.php/Laser_Cutter
* http://www.shapeoko.com/wiki/index.php/CAM#2D_.28Laser_or_plasma_machines.29
* https://hackaday.io/project/4828-raster-2-laser-gcode-generator


# Related work

To develop a complete inventory of fabricatable machines is a goal of the [Fablab Network](http://fablabs.io/).

The [Reprap](http://reprap.org/) aims to build self-replicating machines, where each individual machine can make itself.
Mostly focused on FDM 3d-printers.

