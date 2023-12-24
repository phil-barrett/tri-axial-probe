### PCB section

Schematic for V0.91.

![Schematic V0.91](https://github.com/phil-barrett/tri-axial-probe/blob/main/PCB/V0.90/schematic.png "Schematic V0.91")

## Schematic Description
The ball sensing portion runs at 5V (or less).  A 5V linear regulator is used to take the input power voltage down to run the 74LVC3G14 inverter which provides drive for the LED and output transistors.  The NPN output transistors form a classic pulled high driver. Normally open (NO) and normally closed (NC) outputs are derived from the inverter gates. Current draw with the LED lit is less than 10 mA, allowing it to work without significant heating at up to 28VDC.

## A note on 5V operation.  

When the input voltage is 5V, the 78L05 regulator runs out of spec and delivers a voltage with about 1.2V dropout. This provide 3.8V (or 3.3V with 4.5V input) which powers the 74LVC3G14 within spec.  Since the voltage is restord via the pullups on the output transistors, it all works fine and allows the probe to correctly operate on 5, 12 and 24VCD.  The 74LVC3G14 is specified to run all the way down to a VCC of 2.7V.
