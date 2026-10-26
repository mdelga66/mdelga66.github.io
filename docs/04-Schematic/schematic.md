---
title: Schematic
---

## Overview

Starting with power: a 9 volt barrel jack feeds an LM7805 regulator, with capacitors on the input and output, giving 5 volts. That feeds the Nano’s VBUS pin. The Nano makes its own 3.3 volts, and I take that from the VTG pin to power the mic and op amp, so the signal can never go higher than the PIC’s ADC can handle.

For the mic, a 2.2k resistor from 3.3 volts biases it. A 1 microfarad capacitor blocks DC and passes only the sound. Because I only have a single supply, I build a half-supply reference of about 1.65 volts, called VB, with two 10k resistors and a 10 microfarad capacitor. A 100k resistor ties the op amp input to VB.

The op amp is a non-inverting amplifier. A 47k feedback resistor and a 2.2k resistor in series with a 10 microfarad capacitor to ground give about 22 times gain on audio. DC passes at a gain of one, so the 1.65 volt center stays put. I wired the three unused amplifiers as buffers on VB, so they don’t pick up noise.

The output goes through a 4.7k resistor and a 10 nanofarad capacitor. That’s a low-pass filter at about 3.4 kilohertz, which protects RA0 and reduces aliasing at an 8 kilohertz sample rate.

Last, the 8-pin header: RX on pin 1, TX on pin 2, and ground on pin 8, matching our block diagram. The button on RC4 pulls the pin to ground, and the test LED on RA1 has about a 300 ohm resistor. I put no-connect flags on every unused pin and ran KiCad’s electrical rules check to catch mistakes.


![schematic](screenshotschematic.png){style width:"350" height:"300;"}
**Figure ##:** Showing a example schematic.


## Resouces

The schematic as a PDF download is available [*here*](schematic.pdf)
//#, and the Zip folder of the project [*here*](dummyZip.zip). (not yet)