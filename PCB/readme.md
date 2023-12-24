### PCB section

Schematic for V0.91.

![Schematic V0.91](https://github.com/phil-barrett/tri-axial-probe/blob/main/PCB/V0.90/schematic.png "Schematic V0.91")
The ball sensing portion runs at 5V (or less).  A 5V linear regulator is used to take the input power voltage down to run the 74LVC3G14 inverter which provides drive for the LED and output transistors.  The NPN output transistors form a classic pulled high driver. Normally open (NO) and normally closed (NC) outputs are derived from the inverter gates. 
