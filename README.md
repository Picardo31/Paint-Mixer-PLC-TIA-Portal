# Paint-Mixer-PLC-TIA-Portal
The proyect involves a Paint Company, which needs to implement the project for the automation of the
mixing process for his paint factory, in cans of two different sizes.
The raw material to generate any color is based on the primary colors cyan,
magenta and yellow.

The system will have the following components:

* A pulsating N.C. for emergency.
* Two pulsating N.O. to activate the start of the system and the reset to return to
Operating conditions.
* A selector with three positions for Automatic, OFF and Manual Mode.
* Three tanks of 500 liters each, corresponding to the primary colors
cyan, magenta and yellow.
* A conveyor belt controlled by a three-phase motor.
* A mixer controlled by a three-phase motor and this in turn by a drive
frequency range 0 to 60Hz, driven by 0 -20mA current.
* Five inductive type sensors, located in the positions where it is observed
in the figure.
* Three sonar-type analog level sensors, driven by 0-10V voltage
whose range is from 0 to 500 liters.
* Three solenoid valves of the all or nothing type, to activate or deactivate the dosage
of the primary colors.
* Weight sensor through an analog scale with a range of 0 to 5 kilos,
driven by 0-20mA current.
* Three pilot lights (primary paint can level alarm)
* Two pilot lights to signal the activation of the system and another to indicate a
damage or failure.
* A single-acting pneumatic cylinder, controlled by a solenoid valve
monostable.

System operating conditions:

The automation of the system will allow carrying out the mixing process of cans
of paint of two different sizes (3 and 5 liters), through the implementation of
an HMI.
The process will contemplate two modes of operation:

* Automatic mode.
* Manual mode.

Possible Selection of Colors

![Mix](https://github.com/Picardo31/Paint-Mixer-PLC-TIA-Portal/assets/70179309/c9cceb7e-f9a4-4c8b-81ef-aed835e87dd5)
