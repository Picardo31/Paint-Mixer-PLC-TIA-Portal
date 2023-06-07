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

Automatic Mode:

The system will be activated with a physical or HMI selector, through which the
operator will be able to select Automatic mode.
* Then the size of the paint can to be produced will be selected, 3 or 5 liters.
* It should be considered that the operator may choose any of the colors
or you can generate your own recipe for a custom color.
* It is considered at least two color recipes that are generated from the three
primary colors, for each size of paint pot (in each recipe of the
colors, the amounts of each of the primary colors are considered, as well
such as time and mixer speed).
* In case of choosing a personalized color, the operator will be able to enter
autonomous its own recipe of primary colors to generate a pot of paint,
you will also select the mixing time and mixer speed.
* Once the size of the boat and the desired color (fixed or personalized) have been selected,
the start button will be activated to continue with the process.
The empty 3 or 5 liter can will be located on the conveyor belt, the same as
It will be activated with the start button.
 When the boat is located under the cyan primary color tank, it is detected
by the inductive sensor; and if the recipe requires this color, the appointment is stopped
conveyor, the solenoid valve is activated that will dispense the necessary amount
of that primary color. At the same time the weight scale will be activated
constantly feeling the weight. In the event that the desired color, no
requires any of the primaries located in the tanks, the tape does not
will stop.
* When the paint can has been filled with the necessary weight according to the recipe of the
cyan color, the solenoid valve is closed and the conveyor belt is activated
again, to move the pot to the next primary color.
* The inductive sensor below the magenta primary color is
will activate when the boat has been detected and will stop the tape, as long as
the color recipe calls for this color. By simultaneously opening the solenoid valve and
pouring the necessary amount of said color.
* When the boat has reached the desired weight of this color, the
solenoid valve and activates the conveyor belt again to continue towards
the next tank of paint.
* When the paint can is located under the yellow primary color tank,
is detected by the inductive sensor; and if the recipe calls for this color, it is
stops the conveyor appointment, the solenoid valve is activated that will dispense the
required amount of said primary color. At the same time the weight scale will be
constantly activated by sensing the weight of the boat.
* When the boat has reached the desired weight of this color, the
solenoid valve and activates the conveyor belt again to continue towards
the mixing process.
* When the pot has been filled with the primary colors according to the recipe,
the inductive sensor located under the mixer will detect this and stop the tape
conveyor, which will activate the mixing system after 3s that the
pot under the mixer.
* After 3s, the solenoid valve of the single effect cylinder will be activated, when
fully extended, the mixer will have been located inside the boat
of paint and you are ready to mix.
* Once the mixer is located, it will be activated by time and frequency or
speed according to the selected color recipe. The larger the boat
longer time and speed of the mixing process.
After that time the mixer will stop and deactivate the solenoid valve.
of the single-acting cylinder, thus removing the mixer from the can.
* When the mixer has been completely withdrawn (i.e. the cylinder is
fully contracted), it will take 3s for the ribbon to activate again
conveyor.
* The mixing process ends when the inductive sensor located at the end of the belt
conveyor detects the boat and stops it, so the operator can take the
pot of mixed paint
* In this way the mixing process will be finished, the
production record and the system is ready to start a new
mixing process of the color and size selected above.
* Consider that you should keep track of the number of boats by size and color
that have been generated, as well as the total jackpot count.

EMERGENCY

* By pressing the emergency button, the system will be de-energized by
complete and will stop the mixing process.
* When the emergency has been dealt with and the system is ready to work, the
The operator will press the reset button and enable the system to start a new
mixing process.

SIGNALING AND ALARMS

* The white lamp will light when the system is in
operation, if the machine is in the process of cleaning or filling
tanks, this lamp will be activated intermittently for the duration of said
process.
* The alarm lamps of the three primary paint cans will activate when
the level of the tanks drops to 20% of its total capacity.
* The fault lamp will activate when the emergency button is pressed
and will have intermittent operation, until the service is normalized.
* The HMI will allow to constantly visualize the capacity of the tanks, keep the
production account

Manual Mode:

* Consider a personalized routine to develop the aspects that should be
consider for the operation of the manual mode of the process, which can be
used for cleaning, filling the tanks or acting in an emergency of the
system.

Features:

* 3 liter jar: 4.5kg
* 5 liter container: 8 kg

Variator works as follows:

3 liter jar: time and speed.
* If there is a combination of three primary colors, the mixing time will be
3min.
* The mixing speed will be 30Hz.
* If there is a combination of two primary colors, the mixing time will be
2min.
* The mixing speed will be 15Hz.

5 liter pot: time and speed.
* If there is a combination of three primary colors, the mixing time will be
4min.
* The mixing speed will be 50Hz.
* If there is a combination of two primary colors, the mixing time will be
3min.
* The mixing speed will be 40Hz


Software Developed:

* The program carries out using the TIA PORTAL V14 software and the
PLC S7-1214C., the use of a screen for the compatible HMI will be considered
with said PLC.
* The programming language to be used will be in FBD.
* Linear and structured programming is used.

INTERFACE

* The graphical interface is the KP600 (5-7” A,
6-key color screen or another compatible with the PLC used).
* Four Screens should are considered; for Front Page,
Process, User Management, Signaling, Records, etc.
* An interactive interface is developed in which the change can be evidenced.
status (activated/deactivated) of the inputs and outputs (sensors, valves,
motors, lamps, etc.) the closest thing to the industrial environment to be automated.
* The total and partial production parameters (cans of
3 and 5 liters), primary color tank levels, mixer speed and time, batch production time, current sensor values or
actuators etc
* The interface displays when there is an alarm and display an indicative text
of the specific alarm that has occurred (stop button, motor protection,
or mixer, tank levels, etc.).


Possible Selection of Colors

![Mix](https://github.com/Picardo31/Paint-Mixer-PLC-TIA-Portal/assets/70179309/c9cceb7e-f9a4-4c8b-81ef-aed835e87dd5)

Recipe Selection

![Remt](https://github.com/Picardo31/Paint-Mixer-PLC-TIA-Portal/assets/70179309/bce59e8e-56b8-4e49-8123-d81446bb607c)

Visual Interface of automation of a paint mixing system

![MFT](https://github.com/Picardo31/Paint-Mixer-PLC-TIA-Portal/assets/70179309/5ebe6f15-da13-4f3c-8cfe-1047a702aab6)
