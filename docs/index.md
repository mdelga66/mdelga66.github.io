---
title: Welcome
tags:
- tag1
- tag2
---
<center>
<font size= "6">Mateo Delgado Datasheet</font><br>
as part of<br>
<font size= "8"> RadioLink</font><br>
for<br>
<font size= "5"> Team 105 </font><br>

**Submission: 10/29/2026** <br>
[RadioLink Main Website](https://asu-egr304-2026-f-105.github.io/EGR304-2026-F-105.github.io/)<br>
</center>

## Introduction

* This datasheet documents the design of my individual subsystem for the Team 105 embedded systems project, from block diagram and component selection through schematic, power budget, PCB, and testing. It records the engineering decisions behind my portion of the system so it can be understood, reproduced, and evaluated.

### Project Summary

* Team 105 is developing RadioLink, a portable, off-grid communication device for when cellular or internet service is unavailable. Each team member builds one subsystem around a PIC18F57Q43 Curiosity Nano, and the boards connect through standardized connectors with a shared ground.
* My subsystem is audio input. A CMC-6027-24T electret microphone captures the user’s voice, and an MCP6004 amplifier stage boosts the signal for the PIC’s analog-to-digital converter. The board runs from a single 3.3 V supply.

### My Contribution

* I am responsible for the microphone subsystem: selecting the components, designing the amplifier circuit, and creating the schematic, PCB, power budget, and test features. The board includes a UART header, a pushbutton, and a test LED to support debugging.
* The following sections cover the block diagram, component selection, bill of materials, schematic, power budget, PCB design, and verification results.

As well as the drop down in the top left for each section. ## Explore This Datasheet

* [Block Diagram](C:\Users\mateo_1j2xewk\Documents\GitHub\mdelga66.github.io\docs\01-Block-Diagram)
* [Component Selection](C:\Users\mateo_1j2xewk\Documents\GitHub\mdelga66.github.io\docs\02-Component-Selection)
* [Bill of Materials](C:\Users\mateo_1j2xewk\Documents\GitHub\mdelga66.github.io\docs\03-BOM)
* [Schematic](C:\Users\mateo_1j2xewk\Documents\GitHub\mdelga66.github.io\docs\04-Schematic)
* [Power Budget](C:\Users\mateo_1j2xewk\Documents\GitHub\mdelga66.github.io\docs\05-Power-Budget)