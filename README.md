# Plymouth Kilobot 2019

This repository will be used to share all resources related to the hand-built Kilobots made at Plymouth University. This readme lists all resources required and outlines the process for reproducing our work using open-source material and software packages.

This project was possible due to the material made open-source by other institutions, most importantly [Harvard University](https://ssr.seas.harvard.edu/kilobots) and [Western Carolina University](https://kilobot.wcu.edu/).

## Contents
* PlymouthKilobot2019.zip - Archived KiCad project file of Kilobot design
* PlymKilobot_Gerbers.zip - Gerbers used to produce this version of the Kilobot
* Kilobot schematic - a reproduction of Harvard and WCU designs
* Bill of materials (BOM)
* Assembly diagrams
* Photos and video for reference


## Requirements
Our Overhead Controller (OHC) was built to a design by Western Carolina University (WCU). Their detailed guide was also used for the programming and control of both the OHC and Kilobots. Therefore to replicate this work will require their material available at [Kilobot @ WCU](https://kilobot.wcu.edu/).

In particular:

* OHC gerber files
* Software folder including Kilobot and OHC firmware
* [KiloGUI](https://github.com/acornejo/kilogui), GUI application for Kilobot control
* [“Maker: A Kilobot Swarm”](https://www.asee.org/public/conferences/64/papers/15441/view)

Please note: this project used a Windows 7 computer, and other systems have not been tested.

### Editing the PCB
KiCad is a free open-source electronic CAD suite which was used to create this Kilobot version. It is not required to access the gerber files, but if you wish to make changes to the design, it is available from [KiCad EDA](http://kicad-pcb.org/). 

The archived project file can be imported using the "Unarchive project.." option. The included Kilobot.lib is required for certain symbols and footprints, and must be added using the process described here: ["[library tables] are found in the preferences menu of all KiCad subprogramms (preference -> Manage symbol/footprint libraries.)"](https://forum.kicad.info/t/library-management-in-kicad-version-5/14636).

[freeRouting](https://freerouting.org/) was used in conjunction with KiCad to carry out automatic PCB routing for the new design.


## Process
1. Purchase all PCBs and required components using BOMs included here. For the OHC PCB, use WCU gerber files.

2. Following the guide in [“Maker: A Kilobot Swarm”](https://www.asee.org/public/conferences/64/papers/15441/view), install the required software before assembling the OHC and programming its firmware.

3. Assemble the Kilobots using the included assembly diagram and checklists.

4. Continuing with the WCU guide, program Kilobot firmware using a 2x3 header cable. Connection details are given in "Programming Reference.pdf".

5. Install KiloGUI and use the OHC to program a benchmark test onto the Kilobots. These tests can be found in the WCU materials as well as at [Kilobotics](https://www.kilobotics.com/labs) where details of their functions are available.

## Author
Jamie Trump - Postgraduate Student at University of Plymouth, UK

## Links

### Information and Publications
* [Kilobot @ WCU](https://kilobot.wcu.edu/)
* [“Maker: A Kilobot Swarm”](https://www.asee.org/public/conferences/64/papers/15441/view)
* [Kilobotics Labs](https://www.kilobotics.com/labs)

### Software

* [KiloGUI](https://github.com/acornejo/kilogui)
* [KiCad EDA](http://kicad-pcb.org/)
* [freeRouting](https://freerouting.org/)
