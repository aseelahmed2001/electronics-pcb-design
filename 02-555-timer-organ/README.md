# 555 Timer Mini-Organ PCB

A 12-note electronic mini-organ based on a 555 timer oscillator.

This project was completed as part of the *Crash Course Electronics and PCB Design* course and demonstrates schematic capture, PCB layout, routing, component selection, and preparation of PCB manufacturing files using Altium CircuitMaker.

![PCB 3D View](images/pcb_3d.png)

---

## Overview

The circuit generates different musical tones using a 555 timer and a selectable resistor network.

Twelve push buttons are connected to different resistor values, allowing the oscillator frequency to be changed for each musical note from C4 to B4.

The complete project includes:

- Circuit schematic
- 555 timer oscillator
- 12-note resistor selection network
- 5 V regulated power supply
- Transistor output stage
- PCB layout and routing
- PCB 3D model
- Bill of Materials
- Gerber files
- NC drill files

---

## Tools Used

- Altium CircuitMaker
- PCB schematic capture
- PCB layout and routing
- Design Rule Checking
- Gerber generation
- BOM generation

---

## Circuit Architecture

The circuit consists of four main sections:

1. Power supply and voltage regulation
2. 555 timer oscillator
3. Note-selection network
4. Output driver stage

---

## Power Supply

The circuit uses a 9 V battery input.

A 5 V low-dropout regulator provides the regulated supply voltage for the circuit.

The power section also includes:

- Main power switch
- Input and output capacitors
- 5 V power indicator LED
- VCC test point
- Ground test point

---

## 555 Timer Oscillator

An LMC555 timer is used as the main oscillator.

The oscillator frequency is controlled using a fixed timing resistor, timing capacitor, and a selectable resistor network.

Different resistor values are selected using push buttons to generate different musical tones.

---

## Note Selection

The circuit provides 12 notes covering C4 to B4.

| Note | Target Frequency | Timing Resistor |
|------|-----------------:|----------------:|
| C4 | 261.63 Hz | 27.0 kΩ |
| C#4 / Db4 | 277.18 Hz | 25.5 kΩ |
| D4 | 293.66 Hz | 24.0 kΩ |
| D#4 / Eb4 | 311.13 Hz | 22.1 kΩ |
| E4 | 329.63 Hz | 21.0 kΩ |
| F4 | 349.23 Hz | 20.0 kΩ |
| F#4 / Gb4 | 369.99 Hz | 18.7 kΩ |
| G4 | 392.00 Hz | 17.8 kΩ |
| G#4 / Ab4 | 415.30 Hz | 16.5 kΩ |
| A4 | 440.00 Hz | 16.0 kΩ |
| A#4 / Bb4 | 466.16 Hz | 15.0 kΩ |
| B4 | 493.88 Hz | 14.0 kΩ |

Each push button selects one of these timing resistors and changes the oscillator frequency accordingly.

---

## Output Stage

The oscillator output is connected to a transistor-based output stage using a 2N3904 NPN transistor.

The output section also contains:

- Coupling capacitor
- Biasing resistors
- Output connector
- Flyback protection diode
- Supply decoupling capacitor

---

## Schematic

The complete schematic was created in Altium CircuitMaker.

![555 Timer Mini-Organ Schematic](images/schematic.png)

The schematic includes the complete power, oscillator, note-selection, output, and test-point circuitry.

---

## PCB Design

The schematic was transferred to the PCB layout environment where the components were placed and routed.

The PCB design process included:

- Component placement
- Footprint assignment
- Signal routing
- Power routing
- Ground routing
- Top and bottom copper layers
- Design Rule Checking
- PCB 3D inspection

### Top Layer

![PCB Top Layer](images/pcb_top_layer.png)

### Bottom Layer

![PCB Bottom Layer](images/pcb_bottom_layer.png)

---

## 3D PCB Model

The completed PCB layout was inspected using the 3D visualization environment in CircuitMaker.

![PCB 3D View](images/pcb_3d.png)

The 3D view provides a visual check of component placement, orientation, spacing, and the overall board layout.

---

## Test Points

Test points were included in the design for:

- **VCC** – regulated supply voltage
- **GND** – ground reference
- **Signal** – oscillator/output signal

These provide convenient measurement locations during PCB testing and debugging.

---

## Manufacturing Files

Manufacturing outputs were generated from the completed PCB design.

The repository contains:

- Gerber files
- NC drill files
- Bill of Materials

Gerber files:

`manufacturing/gerber/`

NC drill files:

`manufacturing/nc-drill/`

Bill of Materials:

`manufacturing/BOM_555_Timer.xlsx`

---

## Repository Structure

```text
02-555-timer-organ/
│
├── README.md
│
├── design-files/
│   ├── 555_Timer_Schematic.SchDoc
│   └── 555_Timer_PCB.CMPcbDoc
│
├── manufacturing/
│   ├── gerber/
│   ├── nc-drill/
│   └── BOM_555_Timer.xlsx
│
└── images/
    ├── schematic.png
    ├── pcb_top_layer.png
    ├── pcb_bottom_layer.png
    └── pcb_3d.png
