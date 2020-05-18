# OpenKilo

This repository contains resources related to the OpenKilo Kilobot revision, which was designed to aid repair and extensibility of the Kilobot platform.

This project was possible due to the material made open-source by other institutions, most importantly [Harvard University](https://ssr.seas.harvard.edu/kilobots) and [Western Carolina University](https://kilobot.wcu.edu/).


## Contents

* [Hardware Design](Hardware%20Design/) - KiCad project and exported Gerber files used to produce this version of the Kilobot
* [Documentation](Documentation/) - hardware schematic (produced from Harvard and WCU designs), assembly and programming guides, and bill of materials
* [Photos and Video](Photos%20and%20Video/) - showing the completed robots and their usage


## Requirements

Our Overhead Controller (OHC) was built to a design by Western Carolina University (WCU). Their detailed guide was also used for the programming and control of both the OHC and Kilobots. For more details, refer to their material at https://kilobot.wcu.edu/.

In particular:

* OHC Gerber files
* Software folder including Kilobot and OHC firmware
* [KiloGUI](https://github.com/acornejo/kilogui), GUI application for Kilobot control
* ["Maker: A Kilobot Swarm"](https://www.asee.org/public/conferences/64/papers/15441/view)

### Editing the PCB
KiCad EDA is a free open-source electronic CAD suite which was used to create the OpenKilo design, available from http://kicad-pcb.org/. KiCad is required in order to make changes to the design, but the exported Gerber files are also available for use directly.

The included Kilobot.lib is required for certain symbols and footprints, and must be added to the KiCad project using the process described [here](https://forum.kicad.info/t/library-management-in-kicad-version-5/14636).

[freeRouting](https://freerouting.org/) was used in conjunction with KiCad to carry out automatic PCB routing for the current design.


## Build Process
1. Purchase all PCBs and required components using BOMs included here. For the OHC PCB, use WCU Gerber files.

2. Following the guide in ["Maker: A Kilobot Swarm"](https://www.asee.org/public/conferences/64/papers/15441/view), install the required software before assembling the OHC and programming its firmware.

3. Assemble the OpenKilo hardware using the included assembly diagram and checklists.

4. Continuing with the WCU guide, program Kilobot firmware using a 2x3 header cable. Connection details are given in [Programming Reference.pdf](Documentation/Programming%20Reference.pdf).

5. Install KiloGUI and use the OHC to program a benchmark test onto the OpenKilo robots. These tests can be found in the WCU materials as well as at [Kilobotics](https://www.kilobotics.com/labs) where details of their functions are available.


## Author
The main OpenKilo design and prototyping was completed by Jamie Trump while a postgraduate student at the [University of Plymouth](https://www.plymouth.ac.uk/).

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/).


## Links

### Information and Publications
* [Kilobot @ WCU](https://kilobot.wcu.edu/)
* [“Maker: A Kilobot Swarm”](https://www.asee.org/public/conferences/64/papers/15441/view)
* [Kilobotics Labs](https://www.kilobotics.com/labs)

### Software
* [KiloGUI](https://github.com/acornejo/kilogui)
* [KiCad EDA](http://kicad-pcb.org/)
* [freeRouting](https://freerouting.org/)
