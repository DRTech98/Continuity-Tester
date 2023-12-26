# Continuity-Tester
Continuity Tester Using An 4N35 Optocoupler
This circuit was based on the Encyclopedia of Electronic Circuits Volume 7 circuit from page 468 where a circuit is shown that can test the continuity of resistors, LEDS, and PN junctions of diodes and transistors.

The circuit is fairly simple in that a voltage source is required at the input and output and the input needs a return path in order for the output to work for the given circuit. The LED or buzzer will not turn on until the input has the 9V supply and pin 2 is connected to ground. 

An optocoupler has an Infrared LED light inside that emits light when current flows from anode to cathode, this light then activates the phototransistor inside, which allows current to flow from collector to emitter, thus completing the circuit and either activating the LED or buzzer depending on the position of the switch. 

The switch used is a single pole double throw (SPDT), which means that either position part of the circuit will be activated so long as the input side of the optocoupler has a return path to ground. 

This circuit requires an understanding of both diodes and npn transistors, two components that are used extensively in electronics, and is a good exercise as to the importance of return paths and using a transistor as a switching device. 

The PCB is a 2 layer board with components taken directly from the breadboard prototype and the whole project only took a few hours, as it is very simple and straightforward to understand.

Update (12/26/23): Version 1 of the project had several issues, primarily with the routing in regards to R1, R2, and the capacitor. Due to R1s inscorrect placement, 9V was being feed directly into the base pin of the optocoupler (pin 6), causing the IC to overheat and for the tester to only work for the first initial switches. 

I redid the schematic on the breadboard, and followed each wire piece by piece when making the PCB, version 3 just got ordered, and version 2 had a similar issue with R1 and incorrect routing. A video will be posted showing the working PCB and size comparison and routing differences between the three versions.
