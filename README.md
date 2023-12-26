# TriAxial Probe

This is a project to create an open hardware 3D probe for DIY CNC people. We have a goal of providing the basic design and instructions for building. See below for complete project goals.  Component kits may be available. 

Current status 12/24/2023

The first cut of the PCB, V0.90, has been built and tested. A second version, V0.91, has been sent out for fabrication.  It moves the sensing balls closer together, increases the center hole size to allow a larger spider arbor and adds 2 mounting holes.
![V0.91 PCB](https://github.com/phil-barrett/tri-axial-probe/blob/main/images/3D%20Probe%20V0.91.png "V0.911 PCB")

Here is the first version of the probe, V0.91, exploded to see the internal components. The barrel that holds it together is omitted for clarity. This is a work in progress so it will change.
![V0.91 Exploded](https://github.com/phil-barrett/tri-axial-probe/blob/main/images/probe%20exploded%20V0.91.png "V0.91 Exploded")

The heart of the TriAx probe is the Spider Core that uses the sensing balls as part of a switch.  Lateral or vertical force on the probe tip will cause the spider pins to lift off the balls and break contact.  The PCB circuit is designed to turn this into NO and NC signals.
![V0.91 Spider Core Exploded](https://github.com/phil-barrett/tri-axial-probe/blob/main/images/spider%20core%20exploded.png "V0.91 Spider Core Exploded")



## Project Goals

1. Create an easy to make design for CNC enthusiasts/hobbyists.
2. Machinable on hobby level CNC mills/routers.
3. Costs less than $75 (need to sanity check this).
4. Accuracy better than 0.1mm (need sanity check, can we do better?).
5. Allow use of higher accuracy components, especially probe tips.
6. Usable with common CNC controllers including (but not limited to) Mach 3, Mach 4, Grbl, grblHAL, LinuxCNC.
7. Support for height map probing.
8. Usable with 6 to 24V input power. Stretch goal of supporting 5V.
